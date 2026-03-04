---
title: "Particle Physics & ML Research"
description: "Explore Knut Zoch’s research in experimental particle physics at CERN, with a focus on top quarks, ATLAS, and machine learning."
permalink: /research/
layout: archive
---

My research explores the fundamental nature of matter and energy using the ATLAS experiment at the Large Hadron Collider. I focus on precision measurements involving the top quark, the development of machine learning techniques for particle physics, and searches for new phenomena beyond the Standard Model.

**[↓ Jump to my latest research articles](#research-articles)**

---

## Research Philosophy

I’m drawn to questions at the edge of what’s measurable — rare processes that test theoretical predictions or hint at new physics. I believe the most exciting results come from combining precision measurements with new methodological tools.

Rather than choosing between rigorous analysis and computational innovation, I build strategies that integrate both: algorithms that respect physical symmetries, analyses that extract subtle signals from difficult final states, and collaborative work that brings diverse expertise together.


## Current Research Focus

#### Top-Quark Physics and Precision Measurements

Top-quark measurements provide a window into electroweak interactions at the highest energy scales. My recent work focuses on rare production modes, such as top-quark pairs with additional heavy-flavor jets, which test QCD in new regimes and have revealed persistent discrepancies with theory.

These measurements also provide valuable input for **Effective Field Theory (EFT)** interpretations, constraining new physics effects through a model-independent framework that complements direct searches.

#### Machine Learning Applications

I develop machine learning techniques tailored for collider physics — from conditional normalizing flows that reconstruct invisible particles like neutrinos to graph neural networks for jet tagging and transformers for particle identification.

A central theme is **physics-informed ML**: models that respect detector geometry, symmetry constraints, and physical priors, while providing interpretable and reliable outputs. These tools improve statistical precision and open new avenues for reconstruction and anomaly detection.

#### Searches for New Physics

Much of my search work focuses on model-independent approaches — particularly anomaly detection and long-lived particle signatures. These searches often challenge conventional triggers and reconstruction tools, requiring new techniques from both the detector and algorithmic side.

I'm especially interested in signatures that could go unnoticed in traditional searches: displaced vertices, unusual jet substructure, or unexpected correlations in final states.

---

## Collaboration and Leadership

Working within the ATLAS Collaboration has shaped my scientific approach. I’ve held several leadership roles that combine coordination, mentorship, and technical responsibility:

- **Top Quarks + X convener** (2023–2025): Coordinated precision measurements and new-physics searches involving over 140 collaborators across 20 analyses.
- **Online Data Quality Coordinator** (2021–2023): Oversaw detector monitoring operations during LHC data taking, leading a rotating team of 120 contributors.
- **Machine Learning Liaison** (2021–2023): Supported the top-quark physics group in applying ML techniques and helped shape ML education within the collaboration.

I’ve also supervised students on a range of projects that combine physics and machine learning — from anomaly detection in jet data to reconstructing neutrinos with normalizing flows. For more on this aspect of my work, see the [teaching & mentoring page](/teaching/).

---

## Research Articles

{% assign blog_posts = site.posts | sort: "date" | reverse %}

<div class="research-article-list">
  {% for post in blog_posts %}
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

<br>
