---
title: "Controllable Unsupervised Image Generation (PhD Research)"
excerpt: "Unsupervised GAN architecture for content-style disentanglement enabling image style transfer, domain translation, and attribute manipulation — without label supervision."
collection: portfolio
permalink: /projects/controllable-gan/
date: 2018-09-01
---

**Soongsil University — 2018–2023**

The core question in my PhD was: how do you teach a model to separate *what* something is from *how it looks*, when you have no labels telling it which is which?

This comes up everywhere — style transfer, domain adaptation, attribute editing — but most approaches cheat a little by using paired data, explicit domain labels, or both. I wanted to do it without any of that. The approach I settled on combines an adversarial architecture with a mixing regularization strategy: if you swap the style component between two images, the model should still produce something coherent and content-consistent. That constraint, applied consistently during training, is enough to push real disentanglement to emerge on its own.

On top of that, I developed a projection encoder that gives the latent space some structure — so you can interpolate between styles, transfer the look of one image onto the content of another, or manipulate specific attributes, without the outputs collapsing. A lot of GAN latent spaces are technically disentangled but practically unusable because the geometry is a mess. The projection approach helps with that.

Font synthesis was the main application, because it's a clean testbed: the content is the letterform, the style is the typographic treatment, and the distinction between the two is precise enough that you can actually measure whether your disentanglement is working. The same ideas extend naturally to faces, textures, and other domains where content and appearance are separably defined.

**Publications:**
- Hassan, A. U., Lee, H., & Choi, J. *Exploiting mixing regularization for truly unsupervised font synthesis.* Pattern Recognition Letters, 169, 35–42. (2023)
- Hassan, A. U., Memon, I., & Choi, J. *Learning font-style space using style-guided discriminator for few-shot font generation.* Expert Systems With Applications, 242, 122817. (2024)

**Dissertation:** *Unsupervised Image Generation for Multiple Domains based on Mixing Regularization and Projection Encoder* (Soongsil University, 2023)

**Stack:** PyTorch · GANs · Contrastive Learning · Metric Learning
