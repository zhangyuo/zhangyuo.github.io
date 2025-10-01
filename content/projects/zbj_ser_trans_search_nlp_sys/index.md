---
title: ZBJ Service Transaction Search & NLP System
date: 2017-04-01
links:
  - type: site
    url: https://github.com/yourrepo/zbj-service-search
tags:
  - NLP
  - Text Classification
  - Knowledge Graph
---

**Project Background:**
* Developed a service transaction search system for ZBJ.com, a leading service intermediary platform connecting enterprises with talent providers.
* Addressed challenges of long and noisy user search queries that affected category prediction accuracy and service recommendation.
* Aimed to improve search recall, class prediction, and revenue through automated text intelligence.

**Data Collection & Processing:**
* Source: User search logs and demand orders from ZBJ platform.
* Data cleaning: Removed special symbols, duplicated sentences, and irrelevant text.
* Text segmentation: Customized dictionary segmentation using Ansj.
* Labeling: Combined manual annotation with automated pre-labeling for named entity recognition (NER) and category classification.
* Data augmentation: Supplemented domain-specific vocabulary and knowledge from external sources (e.g., Baidu Encyclopedia).

**Modeling & Optimization:**
* **Named Entity Recognition (NER):**
  - Algorithms: HMM, CRF, LSTM-CRF.
  - Training Tricks: CRF++ tool with feature templates (Unigram/Bigram), L2 regularization tuned via cross-validation, gradient optimization using L-BFGS, Viterbi decoding for sequence labeling.
  - Challenges: Ambiguous token segmentation and unseen words; solutions included custom dictionary expansion and iterative corpus updates.
  - Result: CRF entity recognition accuracy 80.51%, service category prediction improved by 6%.

* **Text Classification:**
  - Algorithms: Naive Bayes, CNN, RNN.
  - CNN Implementation: Word embeddings (Word2Vec), convolutional kernels (length 2-8), max-pooling layers, batch normalization, dropout.
  - RNN Implementation: Sequence padding, dropout on hidden layers, gradient clipping.
  - Optimization: Adjusted hyperparameters including learning rate, batch size, hidden layer depth, neuron count, activation functions, and softmax output.
  - Challenges: Class imbalance and likelihood distribution issues; solutions included data resampling, TF-IDF weighted class probability adjustment, ensemble voting.
  - Result: Naive Bayes accuracy 90%, CNN 85%, RNN 87%.

**Project Workflow:**
1. Preprocess user search queries and order texts.
2. Extract named entities and keywords (themes, regions, industries, requirements).
3. Predict demand category using ensemble of Naive Bayes, CNN, and RNN.
4. Integrate prediction results to improve search ranking and recommendation.
5. Apply results to self-operated business traffic optimization.

**Project Outcome:**
* Optimized search recall and recommendation, directly increasing self-operated traffic revenue by approximately 1 million RMB.
* Enabled precise matching between user queries and service providers.
* Provided a scalable NLP framework for ongoing search engine and recommendation system improvement.

<!--more-->
