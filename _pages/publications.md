---
title: "Publications in Physics & ML"
description: "A selection of Knut Zoch’s publications in particle physics and machine learning, including ATLAS results and interdisciplinary collaborations."
permalink: /publications/
layout: single
---

My work in experimental particle physics has contributed to a wide range of publications — from precision measurements within the ATLAS Collaboration to method-oriented studies on machine learning and anomaly detection. These papers reflect the diversity of my research, spanning collider phenomenology, event reconstruction, and statistical modeling.

As a member of the [ATLAS Collaboration](https://atlas.cern/), I have co-authored over **600 publications**, while contributing directly to a focused set of key analyses, particularly in top-quark physics, event reconstruction, and searches for new physics. Beyond ATLAS, I have published multiple **independent projects** on machine learning and data analysis techniques in high-energy physics.

📚 **Complete publication list** available via:
[Google Scholar](https://scholar.google.com/citations?user=MJ0Q724AAAAJ&hl=en) &#124;
[InspireHEP](https://inspirehep.net/authors/1508982) &#124;
[ORCID](https://orcid.org/0000-0003-2138-6187).


## ATLAS Publications

These papers are part of my collaborative work within the ATLAS experiment at CERN. While many are large-scale efforts, I’ve made **substantial personal contributions** to several key publications — especially those tied to my research on rare top-quark processes and searches for new physics signatures.

{% assign atlas_pubs = site.publications | where: "pub_category", "ATLAS" | sort: "pub_date" | reverse %}
{% for pub in atlas_pubs %}
  {% include publication-entry.html pub=pub render_content=false %}
{% endfor %}


## Independent and Methodological Work

This section features peer-reviewed publications and open resources I’ve led or co-led outside the ATLAS collaboration. These projects focus on **machine learning**, event reconstruction, open datasets, and anomaly detection, bridging physics with broader computational challenges.

{% assign other_pubs = site.publications | where: "pub_category", "individual" | sort: "pub_date" | reverse %}
{% for pub in other_pubs %}
  {% include publication-entry.html pub=pub render_content=false %}
{% endfor %}

---

*These publications illustrate the range and impact of my research — from high-precision collider measurements to innovative methodological work. For context on how these efforts fit into my broader program, see the [Research](/research/) page.*

**Interested in collaboration or have questions about a specific paper?** Feel free to [get in touch](/contact/).
