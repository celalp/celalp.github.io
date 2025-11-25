---
layout: single
title: "Talks"
permalink: /talks/
author_profile: true
talks:
  # - title: "Talk Title"
  #   venue: "Venue Name"
  #   date: 2024-01-01
  #   link: "#"
---

{% for talk in page.talks %}
## {{ talk.title }}
**Venue:** {{ talk.venue }} · **Date:** {{ talk.date }}

[Link]({{ talk.link }})

---
{% endfor %}