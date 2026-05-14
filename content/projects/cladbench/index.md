---
title: 'CLADBench — Collaborative Learning in Graph Anomaly Detection'
date: 2025-01-01
summary: An open-source, publication-grade benchmark unifying tabular, CV, and graph anomaly detectors under a collaborative learning framework with a pseudo-label exchange mechanism.
tags:
  - Graph Neural Networks
  - Semi-Supervised Learning
  - Anomaly Detection
  - LLMs
links:
  - type: code
    url: https://github.com/SafiUllahAdam/CLADBench_02_main
featured: true
---

**CLADBench** is my M2 thesis project at the LIRIS laboratory (GOAL team), under the supervision of Prof. Hamida Seba — an open-source, publication-grade benchmark for **Collaborative Learning in Graph Anomaly Detection**.

<!--more-->

The project unifies three influential ecosystems — **ADBench** (tabular anomaly detection), **GADBench** (supervised graph anomaly detection), and **PyGOD** (unsupervised graph anomaly detection) — under a single collaborative learning framework.

The core scientific contribution is a **pseudo-label exchange mechanism** that lets heterogeneous detectors (tabular, CV-as-tabular, and graph-based) iteratively teach each other on unlabelled data, simulating multi-agent semi-supervised learning. To aggregate the noisy signals these models produce, I designed two neural judge models:

- A **GRU-based judge** for tabular streams.
- An **attention-based recurrent GNN judge** that combines detector embeddings with high-confidence pseudo-labels to produce ensemble anomaly scores on graph data.

The benchmark is engineered to be hospital-grade and reproducible, evaluated with AUC and AP metrics, and intended for direct publication. The work spans semi-supervised learning, graph neural networks, pseudo-labelling, domain generalisation, representation learning, and the use of LLMs for text-to-graph data conversion.
