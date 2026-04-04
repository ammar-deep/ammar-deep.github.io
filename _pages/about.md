---
permalink: /
title: ""
excerpt: "Postdoctoral Researcher in Computer Vision and AI"
author_profile: true
show_title: false
---

<div class="intro-text" markdown="1">

I'm an AI engineer and researcher, currently working as a Postdoctoral Researcher at the [University of Galway](https://www.universityofgalway.ie/) on the ATHENA project. The project focuses on detecting drunk and impaired drivers using multimodal sensors — primarily thermal IR cameras — and deploying the resulting models on edge devices.

My PhD was at [Soongsil University](https://www.ssu.ac.kr/eng/) in Seoul, where I worked on generative adversarial networks for domain translation, style transfer, and character skeletonization. After graduating I joined [DeltaX.ai](https://deltax.ai/) in Seoul, building computer vision systems for the automotive industry: in-cabin monitoring (ICMS), advanced driver assistance (ADAS), and smart factory inspection.

More about my background and research is on the [About](/about/) page.

</div>

---

## News

{% assign news_items = site.data.news | sort: "date" | reverse %}
{% assign hidden_count = news_items.size | minus: 3 %}
<div class="news-list">
{% for item in news_items %}
  <div class="news-item{% if forloop.index > 3 %} news-item--extra{% endif %}">
    <div class="news-item__inner">
      <span class="news-badge">{{ item.date }}</span>
      <span class="news-text">{{ item.text }}</span>
    </div>
  </div>
{% endfor %}
</div>
{% if hidden_count > 0 %}
<button class="news-toggle-btn" id="news-toggle" data-count="{{ hidden_count }}">Show {{ hidden_count }} more &darr;</button>
<script>
(function () {
  var btn = document.getElementById('news-toggle');
  var extras = document.querySelectorAll('.news-item--extra');
  var count = btn.getAttribute('data-count');
  btn.addEventListener('click', function () {
    var open = btn.getAttribute('data-open') === '1';
    extras.forEach(function (el) {
      el.style.maxHeight = open ? '0' : el.scrollHeight + 'px';
    });
    btn.setAttribute('data-open', open ? '0' : '1');
    btn.innerHTML = open ? 'Show ' + count + ' more &darr;' : 'Show less &uarr;';
  });
}());
</script>
{% endif %}
