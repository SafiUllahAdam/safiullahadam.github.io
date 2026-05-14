---
title: 'Multilingual Word Embeddings — English–French Alignment'
date: 2026-03-01
summary: Aligned English–French embedding spaces via orthogonal Procrustes mapping over the MUSE dictionary, validated by a language-identification classifier at ~97% accuracy.
tags:
  - Natural Language Processing
  - Word Embeddings
  - Cross-Lingual NLP
links:
  - type: code
    url: https://github.com/SafiUllahAdam/Multilingual_Embeddings_nlp-
---

I built and aligned **English–French embedding spaces** using Word2Vec, FastText, and pretrained GloVe (6B) representations — FastText chosen for alignment due to its subword-aware robustness to out-of-vocabulary words.

<!--more-->

I implemented an **orthogonal Procrustes mapping** over the MUSE bilingual dictionary to project English vectors into French semantic space, conducted linguistic analyses on synonymy, antonymy, polysemy, and OOV coverage, and validated the aligned space through a downstream language-identification classifier that achieved **~97% accuracy, precision, recall, and F1-score**.

The work confirmed that aligned distributional embeddings preserve meaningful cross-lingual linguistic structure.
