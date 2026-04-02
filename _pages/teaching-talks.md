---
layout: archive
title: "Teaching and Talks"
permalink: /teaching-talks/
author_profile: true
show_title: false
---

{% include base_path %}

<div class="notice--primary">
  This page collects selected teaching, invited tutorials, and research presentations.
</div>

## Teaching

{% for post in site.teaching reversed %}
  {% include archive-single.html %}
{% endfor %}

## Talks and Presentations

{% for post in site.talks reversed %}
  {% include archive-single-talk.html %}
{% endfor %}
