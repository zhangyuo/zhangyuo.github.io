---
title: Luyipai Asset & User Matching System
date: 2018-07-30
links:
  - type: site
    url: https://github.com/yourrepo/luyipai-matching
tags:
  - Recommendation
  - User Profiling
  - Matching System
  - Financial Technology
---

**Project Background:**
* Developed a precise asset-to-investor matching system for Luyipai, a special asset trading platform under Ping An.
* Objectives: Improve user satisfaction, asset transaction conversion, and personalized recommendation.

**Data Collection & Processing:**
* Asset data: Property, mortgage, and financial assets; processed for static and dynamic features.
* User data: Behavioral logs, registration info, and preference settings.
* Data cleaning and tagging for both users and assets.

**Modeling & Optimization:**
* User profiling: Long-term and short-term profile construction.
* Multi-channel asset recall:
  - Single-dimension label-based retrieval.
  - Similar assets retrieval.
  - Collaborative user-based recall.
* Ranking: Linear weighting model, tag relevance score.
* Workflow engineering: Redis for short-term profiles, MySQL/Redis for long-term, Elasticsearch for asset storage.

**Project Workflow:**
1. Construct asset and user profiles with feature scoring.
2. Multi-channel asset recall and top-K selection.
3. Merge and re-rank recalled assets.
4. Provide recommendations and generate detailed asset analysis reports.

**Project Outcome:**
* Built a complete matching system from scratch, significantly improving asset exposure and transaction success rates.
* Detailed reports facilitated user decision-making and increased revenue.

<!--more-->
