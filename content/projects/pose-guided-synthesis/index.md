---
title: 'Pose-Guided Image Synthesis for Human Motion Transfer'
date: 2025-12-01
lastmod: 2026-03-15
summary: Implemented and compared nearest-neighbour retrieval, a vanilla regression network, and a GAN for pose-guided human motion transfer, inspired by Everybody Dance Now.
tags:
  - Computer Vision
  - Generative Models
  - GANs
  - Image Synthesis
---

An academic research project on **Pose-Guided Image Synthesis for Human Motion Transfer**, inspired by *Everybody Dance Now*.

<!--more-->

I implemented and compared three approaches:

- **Nearest-neighbour retrieval** over a pose database.
- A **vanilla neural network** regressing joint coordinates to RGB images.
- A **GAN** for adversarial refinement.

The pipeline used **MediaPipe** for skeleton extraction, **PyTorch** for training, and **OpenCV** for video processing. The project sharpened my understanding of generative modelling, GAN-based image synthesis, intermediate representations, and the trade-offs between realism, generalisation, and visual fidelity.
