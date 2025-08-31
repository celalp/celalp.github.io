---
title: "Papers"
permalink: /papers/
layout: home
collection: papers
entries_layout: home
author_profile: true
---

# My Papers

This page lists all of my published papers.

{% for paper in site.papers %}
  ### [{{ paper.title }}]({{ paper.url | relative_url }})
  <p>{{ paper.excerpt }}</p>
  <p><a href="{{ paper.url | relative_url }}">Read more...</a></p>
  ---
{% endfor %}