---
title: "Knut Zoch | Particle Physics & Machine Learning"
layout: single-skip-h1
permalink: /
header:
  image: "/assets/images/header.jpg"
---

# Knut Zoch – Particle Physicist at CERN

I'm an **experimental particle physicist at CERN**, working with the **ATLAS experiment** at the Large Hadron Collider. My work explores the fundamental laws of nature by studying proton collisions at unprecedented energies. You can read more about my journey in physics on my [about page](/about/).

My [research](/research/) focuses on **top-quark physics**, **machine learning for data analysis**, and **searches for physics beyond the Standard Model**. I design analyses that probe rare processes, uncover subtle patterns in the data, and test the limits of current theoretical models. For technical details on my analyses, you can browse my [publications](/publications/), or check out my [research articles](/research/#research-articles) where I share more in-depth updates on my work.

A central theme in my research is the application of **machine learning**. From identifying invisible particles to spotting unusual events, modern algorithms offer exciting new ways to interpret complex detector data and push science forward.

Beyond the lab, I am deeply committed to **teaching and mentoring**. Whether supervising students on research projects or co-leading interdisciplinary AI courses, helping early-career researchers grow remains one of the most rewarding aspects of my work. Discover more about my approach to supervision and outreach on my [teaching page](/teaching/).

---

### Recent Research Articles

<div class="research-article-list">
  {% assign latest_posts = site.posts | sort: "date" | reverse %}
  {% for post in latest_posts limit:3 %}
    <article class="research-article-item">
      {% if post.header.teaser %}
      <div class="research-article-item__image">
        <a href="{{ post.url | relative_url }}">
          <img src="{{ post.header.teaser | relative_url }}" alt="{{ post.title }}">
        </a>
      </div>
      {% endif %}
      <div class="research-article-item__content">
        <span class="research-article-item__date">{{ post.date | date: "%B %d, %Y" }}</span>
        <h3 class="research-article-item__title">
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h3>
        <div class="research-article-item__excerpt">
          {{ post.excerpt | strip_html | truncate: 500 }}
        </div>
        <a href="{{ post.url | relative_url }}" class="research-article-item__more">Read more &rarr;</a>
      </div>
    </article>
  {% endfor %}
</div>

<div style="margin-top: 1.5em; margin-bottom: 3.5rem;">
  <a href="/research/#research-articles" class="research-article-item__more">View all research articles &rarr;</a>
</div>

---

<p style="font-size: 1.05rem; text-align: center; margin-top: 3em; margin-bottom: 2em;">
  Interested in a collaboration, or have questions about my work or working at CERN?<br>
  Feel free to <strong><a href="/contact/">get in touch</a></strong>.
</p>
