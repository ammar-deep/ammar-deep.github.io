---
permalink: /
title: ""
excerpt: "Postdoctoral Researcher in Computer Vision and Edge AI"
author_profile: true
show_title: false
---

I'm a computer vision researcher and engineer. I did my PhD at Soongsil University in Seoul, spent a couple of years building production AI systems at DeltaX.ai, and I'm now a Postdoctoral Researcher at the [University of Galway](https://www.universityofgalway.ie/) working on the [ATHENA project](https://www.universityofgalway.ie/). For the full story, see the [About](/about/) page.

---

## News

{% assign news_items = site.data.news | sort: "date" | reverse %}
<table class="news-table">
  <tbody>
  {% for item in news_items %}
    <tr>
      <td class="news-date">{{ item.date }}</td>
      <td>{{ item.text }}</td>
    </tr>
  {% endfor %}
  </tbody>
</table>
