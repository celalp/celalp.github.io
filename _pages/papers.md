---
title: "Papers"
permalink: /papers/
layout: home
collection: papers
entries_layout: home
author_profile: true
---

# My Papers

Below is the list of all my peer-reviewed and published papers.

{% for paper in site.papers %}
  <h2>[{{ paper.title }}]({{ paper.url | relative_url }})</h2>
  <p>{{ paper.excerpt }}</p>
  <p><a href="{{ paper.url | relative_url }}">Read more...</a></p>
  ---
{% endfor %}