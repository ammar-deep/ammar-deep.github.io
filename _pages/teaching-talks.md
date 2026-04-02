---
layout: archive
title: "Teaching and Talks"
permalink: /teaching-talks/
author_profile: true
---

{% include base_path %}

## Teaching

{% for post in site.teaching reversed %}
  {% include archive-single.html %}
{% endfor %}

## Talks and Presentations

{% for post in site.talks reversed %}
  {% include archive-single-talk.html %}
{% endfor %}
