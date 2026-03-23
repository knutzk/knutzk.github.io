---
title: "Knut Zoch | Particle Physics & Machine Learning"
layout: single-skip-h1
permalink: /
header:
  image: "/assets/images/header.jpg"
---

# Knut Zoch – Particle Physicist at CERN

I'm a **particle physicist at CERN**, working with the Large Hadron Collider (LHC) – the world’s most powerful particle accelerator. At the LHC, protons collide at unprecedented energies, creating new particles and giving us a glimpse into the fundamental laws of nature. You can read more about my journey into physics on the [about page](/about/).

Within this environment, I am part of the **ATLAS experiment**, one of the major detectors studying these collisions. My [research](/research/) focuses on **top-quark physics**, **machine learning for data analysis**, and **searches for physics beyond the Standard Model**. The top quark, the heaviest known elementary particle, plays a special role in our understanding of nature. By studying how it is produced and how it behaves, we can test the limits of today’s theories and search for new phenomena. The page is also where I regularly share [updates and articles about my work](/research/#research-articles).

Within ATLAS, I work with colleagues to design analyses that probe rare processes and uncover subtle patterns in the data. My projects have included studies of collisions that produce extra heavy quarks as well as the development of new methods that help us interpret the huge amount of information recorded by the detectors. More details can be found on my [publications page](/publications/).

A strong theme in my work is the use of **machine learning**. Modern algorithms help us recognize hidden structures in data that would be hard to detect otherwise. I have applied these techniques to topics ranging from identifying invisible particles to spotting unusual events that could hint at new physics. For me, combining physics and machine learning is one of the most exciting ways to push science forward.

Outside the lab, I enjoy **teaching and mentoring**. I have supervised students on research projects in physics and machine learning, supporting them as they grow into independent researchers. I also co-lead **interdisciplinary machine learning courses** for the German Academic Scholarship Foundation. These courses bring together students from the sciences and humanities to explore algorithms, real-world applications, and the societal dimensions of AI. You can read more about my approach to supervision and outreach on the [teaching page](/teaching/).


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

<p style="font-size: 0.95rem; margin-top: 2em;">
  Interested in a collaboration or have questions about my work? Feel free to <strong><a href="/contact/">get in touch</a></strong>.
</p>
