---
title: "Publications"
seo:
  title: "Publications | Knut Zoch, Ph.D."
  description: "Publication list including ATLAS collaboration papers, methodological innovations, and contributions to particle physics research."
permalink: /publications/
layout: single
---

My research has resulted in numerous publications in leading physics journals, with particular focus on precision measurements, machine learning applications, and methodological innovations in experimental particle physics. As a member of the ATLAS Collaboration, I have co-signed over 600 publications while making direct contributions to key analyses and measurements.

## Publication Overview

**Total Publications:** 600+ as ATLAS Collaboration member<br>
**Direct Contributions:** ~10 publications with substantial personal involvement<br>
**Independent Projects:** Multiple peer-reviewed publications outside the ATLAS collaboration<br>
**Complete List:** [ORCID](https://orcid.org/0000-0003-2138-6187) &#124; [Google Scholar](https://scholar.google.com/citations?user=MJ0Q724AAAAJ&hl=en) &#124; [InspireHEP](https://inspirehep.net/authors/1508982)<br>


## ATLAS Publications

These publications are part of my work within the [ATLAS Collaboration](https://atlas.cern/), one of the largest international research efforts in particle physics. While many are broad collaborative results, I have made direct contributions to key analyses — particularly in top-quark physics and new physics searches.

{% assign atlas_pubs = site.publications | where: "pub_category", "ATLAS" | sort: "pub_date" | reverse %}

{% for pub in atlas_pubs %}
  {% include publication-entry.html pub=pub render_content=false %}
{% endfor %}


## Other Publications

This section highlights publications where I played a leading role in developing new methods, exploring machine learning applications, or contributing to open datasets and software. These works reflect my broader research interests in data analysis and computational physics.

{% assign other_pubs = site.publications | where: "pub_category", "individual" | sort: "pub_date" | reverse %}

{% for pub in other_pubs %}
  {% include publication-entry.html pub=pub render_content=false %}
{% endfor %}

---

*This publication record reflects a comprehensive research program spanning precision measurements, methodological innovations, and collaborative leadership in experimental particle physics.*

**Complete Publication List:** For the most current and comprehensive publication list, please visit one of the following pages: [ORCID](https://orcid.org/0000-0003-2138-6187) &#124; [Google Scholar](https://scholar.google.com/citations?user=MJ0Q724AAAAJ&hl=en) &#124; [InspireHEP](https://inspirehep.net/authors/1508982).

**Collaboration Opportunities:** Interested in research collaboration or have questions about any of these publications? Please [contact me](/contact/) to discuss potential partnerships.

