---
layout: single
permalink: /about/
title: "About"
author_profile: true
show_title: false
---

I'm Ammar — a computer vision researcher and engineer based in Galway, Ireland. I did my PhD at Soongsil University in Seoul, spent a couple of years building real-world AI systems at a startup, and I'm now a postdoc at the University of Galway. Feel free to reach out if anything here overlaps with what you're working on.

<div class="research-areas">
  <span class="area-badge">Thermal DMS</span>
  <span class="area-badge">Vision-Language Models</span>
  <span class="area-badge">Open-Vocab Detection</span>
  <span class="area-badge">Edge AI</span>
  <span class="area-badge">Driver Monitoring</span>
  <span class="area-badge">GANs</span>
  <span class="area-badge">Generative Models</span>
</div>

---

#### What I do

Most of my work sits at the intersection of "making models that actually work" and "making them work on hardware that wasn't designed to run them." I've moved across generative models, driver monitoring, 3D scene understanding, and edge deployment — different problems, but the same underlying interest: vision systems that hold up in the real world.

Right now I'm part of the [ATHENA project](https://www.universityofgalway.ie/), where the focus is on detecting impaired drivers using thermal cameras. A big chunk of my time is benchmarking VLMs — LLaVA, Qwen, Mistral, SmolVLM — on driver monitoring datasets, trying to understand how much genuine scene understanding these models actually have versus how much they're pattern-matching. I'm also looking at open-vocabulary detection frameworks for in-cabin scenes, where you can't always predict in advance what you'll need to find.

#### Before that

At DeltaX.ai in Seoul, I worked on the kind of computer vision that has to run inside a moving car or on a factory floor and can't fail. That meant in-cabin monitoring — seatbelt detection, drowsiness, occupancy, all from IR cameras — road scene segmentation for an ADAS pipeline, and a 27-camera smart factory system written in C++. A lot of my time there was figuring out how to take a model that worked fine on a GPU and make it run on a Jetson or Hailo board without losing what mattered about it.

My PhD was about generative models — specifically, teaching GANs to separate content from style without any labels. No paired data, no domain supervision. The main application was font synthesis, where the problem of disentangling *what a character is* from *how it's drawn* turns out to be a surprisingly rich testbed for unsupervised representation learning.

#### Sensors and tools I work with

I've worked with RGB, fisheye, depth, and IR/thermal cameras across different projects, along with LiDAR, IMU, and CAN bus data. On the software side, PyTorch is my daily driver; I've deployed models through ONNX, TensorRT, and DeepStream onto Jetson, TI, and Hailo hardware. C++ where latency actually matters.

#### Open to collaboration on

Driver monitoring and in-cabin perception, VLM/LLM evaluation for real-world vision tasks, generative models and domain adaptation, and efficient edge AI deployment. If your work touches any of these, I'd love to hear from you.

---

#### Education

- **Ph.D.** Computer Science & Engineering, Soongsil University, Seoul (2018–2023) — advised by [Prof. Jaeyoung Choi](https://scholar.google.com/citations?user=YJ7fWWgAAAAJ&hl=en)
- **M.S.** Computer Science & Engineering, Soongsil University (2016–2018) · International Graduate Research Scholar
- **B.S.** Software Engineering, International Islamic University, Pakistan (2009–2013) · Federal Government Scholar

---

#### Get in touch

Email: [ammar.instantsoft@gmail.com](mailto:ammar.instantsoft@gmail.com)
· [GitHub](https://github.com/ammar-deep)
· [LinkedIn](https://www.linkedin.com/in/ammar-ul-hassan-muhammad-131130171)
· [Google Scholar](https://scholar.google.com/citations?user=OGq4xDYAAAAJ&hl=en)
