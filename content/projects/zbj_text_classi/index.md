---
title: ZBJ Demand Order Text Classification
date: 2017-05-01
links:
  - type: site
    url: https://github.com/yourrepo/zbj-text-classification
tags:
  - NLP
  - Deep Learning
  - CNN
  - RNN

featured: true
---

**Project Background:**
* Designed an automated text classification system for ZBJ.com demand orders.
* Objective: Accurately identify user intent from free-text orders to match relevant service providers.

**Data Collection & Processing:**
* Collected 1M+ demand orders covering 15 primary categories and 100+ tertiary categories.
* Cleaned data: Removed meaningless symbols, repeated sentences, and irrelevant text.
* Text segmentation: Custom dictionary segmentation using Ansj.
* Vectorization: Word2Vec embeddings trained on domain corpus; TF-IDF and BOW for baseline models.
* Labeling: Combined manual annotation with automated heuristics.

**Modeling & Optimization:**
* Algorithms: Naive Bayes, CNN, RNN.
* **CNN Model:**
  - Input: Fixed-length sequences with zero-padding for short orders.
  - Convolutional layers with multiple kernel sizes (2-8), max-pooling, batch normalization.
  - Fully connected layers with dropout and softmax for classification.
* **RNN Model:**
  - Input sequences padded/truncated.
  - LSTM layers with dropout, gradient clipping.
* Hyperparameter tuning: Learning rate, batch size, hidden layer neurons, activation functions, iteration rounds.
* Ensemble strategy: Voting across Naive Bayes, CNN, RNN to improve robustness.

**Workflow:**
1. Preprocess text and remove noise.
2. Apply NER and keyword extraction for feature enrichment.
3. Train models and perform cross-validation.
4. Ensemble predictions for final category output.

**Project Outcome:**
* Naive Bayes accuracy: 90%, CNN accuracy: 85%, RNN accuracy: 87%.
* Improved service provider matching, optimized search engine results, and increased user satisfaction.

<!--more-->
