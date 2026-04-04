---
title: "ATHENA Project: Impaired Driver Detection with Thermal Cameras"
excerpt: "Postdoctoral research on drunk/impaired driver detection using thermal (LWIR) cameras, VLM-based evaluation pipelines, and open-vocabulary detection for driver monitoring."
collection: portfolio
permalink: /projects/athena/
date: 2025-11-01
status: ongoing
organization: University of Galway, Ireland
period: Nov 2025 – Present
tech: "Thermal IR Cameras, VLMs, Open-Vocab Detection, Edge AI, Driver Monitoring, LLaVA, Qwen-VL"
header:
  teaser: images/pub_placeholder.png
---

**University of Galway — 2025–Present**

Detecting an impaired driver is a harder problem than it looks. You're not just watching for closed eyes — you want to catch subtler, earlier signs, and you need a system that works regardless of lighting, time of day, or whether the driver is wearing sunglasses. Thermal cameras help a lot with this, which is the core premise of ATHENA.

My work on the project is split between two threads. The first is benchmarking Vision-Language Models — LLaVA, Qwen-VL, Mistral, SmolVLM, InstructBLIP — on driver monitoring datasets. The question I'm trying to answer is how well these models actually understand in-cabin scenes, and whether our current evaluation methods are telling us anything meaningful. The gap between what these models claim and what they do in a structured benchmark is genuinely interesting, and it's still early days for this kind of work.

The second thread is open-vocabulary detection using YOLO-World and YOLO-E on thermal imagery. The appeal of open-vocabulary detection here is that you're not locked into a fixed class list — useful when you're deploying in the real world and can't anticipate every object or situation in advance.

**Stack:** PyTorch · Thermal / LWIR cameras · YOLO-World · YOLO-E · LLaVA · Qwen-VL · Python

