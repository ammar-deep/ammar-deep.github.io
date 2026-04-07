---
title: "Font Generation Research: Few-Shot, Family Synthesis & Skeletonization"
excerpt: "GAN-based research on few-shot font generation, font family synthesis, and text image skeletonization — with publications in CVPR, Expert Systems with Applications, Knowledge-Based Systems, and IJDAR."
collection: portfolio
permalink: /projects/font-generation/
date: 2021-01-01
status: completed
organization: Soongsil University, Seoul
period: 2018 – 2023
tech: "GANs, Few-Shot Font Generation, Font Family Synthesis, Skeletonization, Style Transfer, CVPR, TensorFlow"
header:
  teaser: images/pub_placeholder.png
---

**Soongsil University — 2018–2023**

Font generation looks like a simple problem until you think about it for more than a minute. A typeface isn't a set of images — it's a design system where every glyph has to be internally consistent across potentially hundreds of characters, in a style that's distinct, learnable, and reproducible from very few examples. That combination of constraints made it a genuinely interesting machine learning problem to work on.

The few-shot work took up most of the research time. The goal was to learn a style latent space that's actually structured — not just a bag of features, but a space where nearby points mean visually similar styles, and where you can reliably transfer a style from a handful of reference characters to a full unseen alphabet. I used metric and contrastive learning objectives to shape that space, and a style-guided discriminator to keep the generator from drifting. This eventually extended to Korean and Chinese scripts, which added a layer of compositional complexity — those writing systems have explicit component structure that Latin fonts don't, and using it turned out to help a lot.

Font family synthesis is a related but distinct problem: given one or a few variants of a typeface, generate the rest of the family. The unpaired setup was a deliberate design choice — it reflects how actual type designers work, where you define a stylistic direction rather than reproduce an existing example. That work ended up as a Korean patent.

The skeletonization work was a collaboration. The idea is that the skeleton of a character — its underlying stroke structure — is a more compact and editable representation than the full glyph. SkelGAN extracts those skeletons end-to-end using a GAN, and SKFont uses them as the basis for a Korean font generator that can produce new glyphs from skeletal guidance rather than pixel-level targets.

**Selected publications:**
- Hassan, A. U., Memon, I., & Choi, J. *Learning font-style space using style-guided discriminator for few-shot font generation.* Expert Systems With Applications, 242, 122817. (2024)
- Hassan, A. U., Lee, H., & Choi, J. *Exploiting mixing regularization for truly unsupervised font synthesis.* Pattern Recognition Letters, 169, 35–42. (2023)
- Hassan, A. U., Memon, I., & Choi, J. *Real-time high quality font generation with conditional GAN.* Expert Systems with Applications, 213, 118907. (2022)
- Hassan, A. U., & Choi, J. *FontNet: Closing the gap to font designer performance in font synthesis.* AI for Content Creation (AI4CC), CVPR 2022.
- Hassan, A. U., Ahmed, H., & Choi, J. *Unpaired font family synthesis using conditional generative adversarial networks.* Knowledge-Based Systems, 229, 107304. (2021)
- Ko, D. H., Hassan, A. U., et al. *SKFont: Skeleton-driven Korean font generator.* IJDAR. (2021)
- Ko, D. H., Hassan, A. U., et al. *SkelGAN: A font image skeletonization method.* Journal of Information Processing Systems. (2021)

**Stack:** PyTorch · TensorFlow · GANs · Metric Learning · Contrastive Learning
