---
layout: single
title: "Alper Celik"
permalink: /
header:
  overlay_color: "#5e616c"
  overlay_filter: "0.3"
  cta_label: "Learn more"
  cta_url: "/about/"
excerpt: "Data scientist & researcher at the intersection of machine learning and biology."
author_profile: true
---

## Recent Papers

{% assign papers_page = site.pages | where: "permalink", "/papers/" | first %}
{% for paper in papers_page.papers limit:3 %}
- [{{ paper.title }}](/papers/#{{ paper.title | slugify }})  
  <small><em>{{ paper.venue }}</em> · {{ paper.date | slice: 0, 4 }}</small>
{% endfor %}

---

## Projects
{% assign projects_page = site.pages | where: "permalink", "/projects/" | first %}
{% for project in projects_page.projects limit:3 %}
- [{{ project.title }}](/projects/)  
  <small>{{ project.description }}</small>
{% endfor %}