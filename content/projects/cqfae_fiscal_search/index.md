---
title: Fiscal Policy Knowledge Graph & Search Engine
date: 2018-06-01
links:
  - type: site
    url: https://github.com/yourrepo/zhongjinsuo-kg-policy
tags:
  - Knowledge Graph
  - Policy Search
  - Neo4j
  - Fiscal Intelligence
featured: true
---

**Project Background:**
* Designed and led the development of a fiscal intelligence system for Zhong Jin Suo, focusing on policy document retrieval and intelligent recommendation.
* Objective: Solve inefficiencies in policy document search and enable deep policy analysis via knowledge graph technology.

**Data Collection & Processing:**
* Built a policy crawler system for scheduled acquisition of fiscal and tax policy documents.
* Structured storage in MySQL and MongoDB; full-text indexing in Elasticsearch.
* Entity & relation extraction:
  - Word2Vec + K-Means for entity discovery.
  - N-Gram + top-down taxonomy construction for category-label hierarchy.
  - LSTM-CRF for fine-grained entity-relation extraction.

**Knowledge Graph Construction:**
* Ontology modeling (services, industries, regions) based on OWL.
* Implemented ontology query with SPARQL; developed region recognition interface for geographic tagging.
* Knowledge graph stored and visualized in Neo4j.

**Modeling & Optimization:**
* Multi-level policy association graphs:
  - **2-level association graph** for related policies.
  - **Tree-structured hierarchy graph** (central, provincial, municipal levels).
* Recommendation:
  - Similarity-based: Jaccard similarity.
  - Hot policy discovery: PageRank centrality.
  - Community detection: Louvain algorithm for policy domain clustering.
* Path discovery:
  - Maximum Spanning Tree (MST) for strong relationship tracing.
  - Dijkstra algorithm for shortest policy association path analysis.
* Policy Q&A:
  - RASA-based intent recognition and slot filling.
  - Query templates mapped to Elasticsearch/MySQL/Neo4j.

**Workflow:**
1. Crawl and parse policy documents, store in databases, index in ES.
2. Extract entities and build ontology-driven knowledge graph in Neo4j.
3. Implement multi-level association queries and recommendation algorithms.
4. Provide Q&A services for fiscal indicators using dialog framework.
5. Visualize policy relationships and enable in-depth policy analysis.

**Project Outcome:**
* Successfully deployed the **Fiscal Intelligence System**, commercialized and sold to government and enterprise clients.
* Reduced policy retrieval time drastically, enabling policy analysts to discover associations and insights efficiently.
* Significantly enhanced fiscal policy research and decision-making processes through intelligent search and graph-based analytics.

<!--more-->
