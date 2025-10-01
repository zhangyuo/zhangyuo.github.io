---
title: ZBJ Service Transaction Knowledge Graph
date: 2017-12-01
links:
  - type: site
    url: https://github.com/yourrepo/zbj-kg-service
tags:
  - Knowledge Graph
  - NLP
  - Service Recommendation
  - User Intent Recognition

featured: true
---

**Project Background:**
* Developed a service transaction knowledge graph for ZBJ.com, China’s leading crowdsourcing and service marketplace platform.
* Objective: Enhance search accuracy, improve user intent recognition, and optimize category classification and recommendation.

**Data Collection & Processing:**
* Data source: Millions of user service requests and transaction orders.
* Text preprocessing: Noise removal, tokenization with domain-specific dictionary, stopword filtering.
* Entity recognition: LSTM-CRF for extracting named entities such as service themes, industries, and geographic regions.
* Taxonomy design: Constructed hierarchical labels for Service → Industry → Region, forming the backbone ontology of the knowledge graph.

**Modeling & Optimization:**
* Knowledge Graph (KG) constructed using Neo4j, linking services, industries, and regions.
* Entity-relationship extraction based on co-occurrence and semantic similarity (Word2Vec + K-Means).
* Service intent classification improved by integrating KG features into Naive Bayes and CNN classifiers.
* Implemented query expansion using KG to capture long-tail user intents.

**Workflow:**
1. Parse user queries and demand order texts.
2. Extract entities and relations using LSTM-CRF and clustering-based methods.
3. Populate KG with service-industry-region ontology.
4. Enhance search retrieval and category classification with KG-driven features.
5. Recommend related services and providers via knowledge graph traversal.

**Project Outcome:**
* Increased user intent recognition accuracy by 8%.
* Improved service category prediction performance and search recall.
* Enabled intelligent service matching, increasing transaction success rate and platform revenue.

<!--more-->
