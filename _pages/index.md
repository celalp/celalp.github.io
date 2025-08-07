---
layout: splash
title: "Alper Celik"
permalink: /
header:
  overlay_color: "#5e616c"
  overlay_filter: "0.3"
  overlay_image: /assets/images/header.jpg  # Optional background image
  cta_label: "Learn more"
  cta_url: "/about/"
  caption: "Welcome to my academic & data science portfolio"
excerpt: "Data scientist & researcher at the intersection of machine learning and biology."
---

## Recent Papers

{% for paper in site.papers limit:3 %}
- [{{ paper.title }}]({{ paper.url | relative_url }})  
  <small><em>{{ paper.venue }}</em> · {{ paper.date | date: "%Y" }}</small>
{% endfor %}

---

## Recent Talks

{% for talk in site.talks limit:3 %}
- [{{ talk.title }}]({{ talk.url | relative_url }})  
  <small><em>{{ talk.event }}</em> · {{ talk.date | date: "%Y" }}</small>
{% endfor %}

---

## Recent Blog Posts

{% for post in site.posts limit:3 %}
- [{{ post.title }}]({{ post.url | relative_url }})  
  <small>{{ post.date | date: "%B %d, %Y" }}</small>
{% endfor %}