---
title: 'PSX-PNR — Personalised News Recommendation for Stock Investors'
date: 2026-01-01
summary: A personalised news recommendation engine for Pakistan Stock Exchange investors, comparing Word2Vec and SBERT embeddings across ~35K headlines and 813K stock-market rows.
tags:
  - Natural Language Processing
  - Recommender Systems
  - Sentence Embeddings
  - Information Retrieval
links:
  - type: code
    url: https://github.com/aserec05/psx-pnr
---

**PSX-PNR** is a personalised news recommendation engine for Pakistan Stock Exchange investors.

<!--more-->

The system compares **Word2Vec** and **SBERT** (MiniLM, MPNet, Multilingual) embeddings across three real financial datasets (~35,000 headlines and 813,000 stock-market rows), constructs user profile vectors from simulated reading histories, and ranks daily news using cosine similarity with optional recency boosting.

Through a rigorous evaluation using **Precision@K** and **NDCG@K**, I showed that SBERT-MPNet produces clear sector-level separation (+0.175 Δ) where Word2Vec collapses financial vocabulary, and that SBERT without recency boosting yields the strongest overall ranking quality.

The project deepened my expertise in sentence embeddings, contrastive retrieval, user modelling, and information-retrieval evaluation metrics.
