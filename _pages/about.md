---
permalink: /
title: ""
excerpt: "Postdoctoral Researcher in Computer Vision and Edge AI"
author_profile: true
show_title: false
redirect_from: 
  - /about/
  - /about.html
---

#### Hi there

I'm Ammar — a computer vision researcher and engineer based in Galway, Ireland. I did my PhD at Soongsil University in Seoul, spent a couple of years building real-world AI systems at a startup, and I'm now a postdoc at the University of Galway. Feel free to look around, and reach out if anything here overlaps with what you're working on.

#### What I do

Most of my work sits at the intersection of "making models that actually work" and "making them work on hardware that wasn't designed to run them." I've moved across generative models, driver monitoring, 3D scene understanding, and edge deployment — different problems, but the same underlying interest: vision systems that hold up in the real world.

Right now I'm part of the [ATHENA project](https://www.universityofgalway.ie/), where the focus is on detecting impaired drivers using thermal cameras. A big chunk of my time is benchmarking VLMs — LLaVA, Qwen, Mistral, SmolVLM — on driver monitoring datasets, trying to understand how much genuine scene understanding these models have versus how much they're pattern-matching. I'm also looking at open-vocabulary detection frameworks for in-cabin scenes, where you can't always predict in advance what you'll need to find.

#### Before that

At DeltaX.ai in Seoul, I worked on the kind of computer vision that has to run inside a moving car or on a factory floor and can't fail. That meant in-cabin monitoring — seatbelt detection, drowsiness, occupancy, all from IR cameras — road scene segmentation for an ADAS pipeline, and a 27-camera smart factory system written in C++. A lot of my time there was figuring out how to take a model that worked fine on a GPU and make it run on a Jetson or Hailo board without losing what mattered about it.

My PhD was about generative models — specifically, teaching GANs to separate content from style without any labels. No paired data, no domain supervision. The main application was font synthesis, where the problem of disentangling *what a character is* from *how it's drawn* turns out to be a surprisingly rich testbed.

#### Education

- **Ph.D.** Computer Science & Engineering, Soongsil University, Seoul (2018–2023) — advised by [Prof. Jaeyoung Choi](https://scholar.google.com/citations?user=YJ7fWWgAAAAJ&hl=en)
- **M.S.** Computer Science & Engineering, Soongsil University (2016–2018)
- **B.S.** Software Engineering, International Islamic University, Pakistan (2009–2013)

#### Get in touch

Email is the best way: [ammar.instantsoft@gmail.com](mailto:ammar.instantsoft@gmail.com). You can also find me on [GitHub](https://github.com/ammar-deep), [LinkedIn](https://www.linkedin.com/in/ammar-ul-hassan-muhammad-131130171), and [Google Scholar](https://scholar.google.com/citations?user=OGq4xDYAAAAJ&hl=en).

---

## News

{% assign news_items = site.data.news | sort: "date" | reverse %}
<table>
  <tbody>
  {% for item in news_items %}
    <tr>
      <td style="white-space:nowrap; padding-right:1.5em;"><strong>{{ item.date }}</strong></td>
      <td>{{ item.text }}</td>
    </tr>
  {% endfor %}
  </tbody>
</table>
