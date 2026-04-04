---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
show_title: false
---

{% include base_path %}

<p style="font-size:0.9em; color:#666; margin-bottom:1.5em;">Full list on <a href="{{ site.author.googlescholar }}">Google Scholar</a>.</p>

{% for post in site.publications reversed %}
  {% include pub-card.html %}
{% endfor %}
