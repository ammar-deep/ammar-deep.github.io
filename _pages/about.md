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

I'm Muhammad Ammar ul Hassan, a Postdoctoral Researcher at the [University of Galway](https://www.universityofgalway.ie/), Ireland. I received my Ph.D. from Soongsil University, Seoul, South Korea. Feel free to reach out if you want to collaborate or just have a chat.

#### What I Do

I am a computer vision researcher and engineer with experience across academic research and industry.

- **Current (2025–):** Postdoctoral researcher on the ATHENA Project — drunk/impaired driver detection using thermal cameras, VLM evaluation for driver monitoring systems, and open-vocabulary object detection for in-cabin understanding.
- **Industry (2023–2025):** AI Engineer at DeltaX.ai — built and deployed real-world systems for in-cabin monitoring (ICMS), ADAS pipelines, and smart factory vision applications.
- **PhD Research (2018–2023):** Deep generative models — domain translation, style transfer, and skeletonization, applied to font synthesis and facial attribute editing.

#### What I'm Working On

- Drunk/impaired driver detection using thermal (LWIR) camera systems.
- Evaluating Vision-Language Models (VLMs) for automated driver monitoring assessment.
- Open-vocabulary object detection for unconstrained automotive scenes.
- Multimodal perception and efficient model deployment on resource-constrained edge devices.

#### Sensors & Tools I Work With

- **Sensors:** RGB, Fisheye, Depth, IR/Thermal cameras · LiDAR · IMU · CAN bus
- **Frameworks:** PyTorch (primary), TensorFlow; deployment experience with embedded vision hardware

#### Looking to Collaborate On

- Automotive safety, driver monitoring, and in-cabin perception.
- VLM/LLM evaluation and adaptation for real-world vision tasks.
- Generative models, domain adaptation, and open-vocabulary recognition.
- Edge AI and efficient deployment for embedded vision systems.

#### Education

- **Ph.D.** in Computer Science & Engineering — Soongsil University, Seoul (2018–2023), supervised by [Prof. Jaeyoung Choi](https://scholar.google.com/citations?user=YJ7fWWgAAAAJ&hl=en)
- **M.S.** in Computer Science & Engineering — Soongsil University (2016–2018) · International Graduate Research Scholar
- **B.S.** in Software Engineering — International Islamic University, Pakistan (2009–2013)

#### How to Reach Me

- Email: [ammar.instantsoft@gmail.com](mailto:ammar.instantsoft@gmail.com)
- [GitHub](https://github.com/ammar-deep) · [LinkedIn](https://www.linkedin.com/in/ammar-ul-hassan-muhammad-131130171) · [Google Scholar](https://scholar.google.com/citations?user=OGq4xDYAAAAJ&hl=en)

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
