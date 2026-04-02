---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
show_title: false
---

<div class="notice--primary">
  Publications are listed from newest to oldest. A full publication list is also available on <a href="{{ site.author.googlescholar }}">Google Scholar</a>.
</div>

{% if site.author.googlescholar %}
  You can also find my articles on <u><a href="{{ site.author.googlescholar }}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
