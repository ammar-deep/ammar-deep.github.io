---
layout: archive
title: "Academic"
permalink: /teaching-talks/
author_profile: true
show_title: false
---

{% include base_path %}

<h4 class="projects-section-heading">Teaching</h4>

{% assign teaching_sorted = site.teaching | sort: "date" | reverse %}
{% for post in teaching_sorted %}
<div class="activity-card">
  <div class="activity-card__icon"><i class="fa fa-graduation-cap" aria-hidden="true"></i></div>
  <div class="activity-card__body">
    <div class="activity-card__title">{{ post.title }}</div>
    <p class="activity-card__meta">
      <span class="activity-card__type">{{ post.type }}</span>
      <span class="activity-card__sep">·</span>
      <span>{{ post.venue }}</span>
      <span class="activity-card__sep">·</span>
      <span>{{ post.date | date: "%Y" }}{% if post.location %}, {{ post.location }}{% endif %}</span>
    </p>
    {% if post.excerpt %}<p class="activity-card__desc">{{ post.excerpt }}</p>{% endif %}
  </div>
</div>
{% endfor %}

<h4 class="projects-section-heading" style="margin-top:2.5em;">Talks &amp; Presentations</h4>

{% assign talks_sorted = site.talks | sort: "date" | reverse %}
{% for post in talks_sorted %}
<div class="activity-card">
  <div class="activity-card__icon"><i class="fa fa-microphone" aria-hidden="true"></i></div>
  <div class="activity-card__body">
    <div class="activity-card__title">{{ post.title }}</div>
    <p class="activity-card__meta">
      <span class="activity-card__type">{{ post.type }}</span>
      <span class="activity-card__sep">·</span>
      <span>{{ post.venue }}</span>
      <span class="activity-card__sep">·</span>
      <span>{{ post.date | date: "%Y" }}{% if post.location %}, {{ post.location }}{% endif %}</span>
    </p>
    {% if post.excerpt %}<p class="activity-card__desc">{{ post.excerpt }}</p>{% endif %}
  </div>
</div>
{% endfor %}

<h4 class="projects-section-heading" style="margin-top:2.5em;">Honors &amp; Awards</h4>

<div class="activity-card">
  <div class="activity-card__icon"><i class="fa fa-trophy" aria-hidden="true"></i></div>
  <div class="activity-card__body">
    <div class="activity-card__title">International Graduate Research Scholarship</div>
    <p class="activity-card__meta">
      <span class="activity-card__type">Scholarship</span>
      <span class="activity-card__sep">·</span>
      <span>Soongsil University, Seoul</span>
      <span class="activity-card__sep">·</span>
      <span>2016 &ndash; 2023</span>
    </p>
    <p class="activity-card__desc">Awarded for both M.S. (2016&ndash;2018) and Ph.D. (2018&ndash;2023) studies, covering full tuition and a monthly stipend.</p>
  </div>
</div>

<div class="activity-card">
  <div class="activity-card__icon"><i class="fa fa-trophy" aria-hidden="true"></i></div>
  <div class="activity-card__body">
    <div class="activity-card__title">Best Paper Bronze Award</div>
    <p class="activity-card__meta">
      <span class="activity-card__type">Award</span>
      <span class="activity-card__sep">·</span>
      <span>International Conference on Smart Media and Applications (SMA)</span>
      <span class="activity-card__sep">·</span>
      <span>2020</span>
    </p>
    <p class="activity-card__desc">Awarded for the Font2Fonts paper presented at SMA 2020, South Korea.</p>
  </div>
</div>

<div class="activity-card">
  <div class="activity-card__icon"><i class="fa fa-trophy" aria-hidden="true"></i></div>
  <div class="activity-card__body">
    <div class="activity-card__title">Federal Government Scholarship</div>
    <p class="activity-card__meta">
      <span class="activity-card__type">Scholarship</span>
      <span class="activity-card__sep">·</span>
      <span>International Islamic University, Islamabad</span>
      <span class="activity-card__sep">·</span>
      <span>2009 &ndash; 2013</span>
    </p>
    <p class="activity-card__desc">Full scholarship for B.S. in Software Engineering.</p>
  </div>
</div>

<h4 class="projects-section-heading" style="margin-top:2.5em;">Patent</h4>

<div class="activity-card">
  <div class="activity-card__icon"><i class="fa fa-file-text-o" aria-hidden="true"></i></div>
  <div class="activity-card__body">
    <div class="activity-card__title">Method and Apparatus for Generating Font Family Using Deep Learning</div>
    <p class="activity-card__meta">
      <span class="activity-card__type">Korean Patent</span>
      <span class="activity-card__sep">·</span>
      <span>No. 2-2006-027849-9</span>
      <span class="activity-card__sep">·</span>
      <span>2022</span>
    </p>
    <p class="activity-card__desc">Hassan, A. U. &amp; Choi, J. &mdash; Soongsil University Industry-Academic Cooperation Foundation.</p>
  </div>
</div>

