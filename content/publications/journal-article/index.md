---
title: "Real-time combustion torque estimation and dynamic misfire fault diagnosis in gasoline engine"
authors:
- Taixiong Zheng
- admin
- Yongfu Li
- Lichen Shi
author_notes:
# - "Equal contribution"
# - "Equal contribution"
date: "2019-07-01T00:00:00Z"

# Schedule page publish date (NOT publication's date).
publishDate: "2019-07-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "*Mechanical Systems and Signal Processing, 126*, 521-535"
publication_short: ""

abstract: In this research, an innovative state observer of gasoline engine based on the combination of Luenberger and sliding mode technique is proposed. This state observer is designed to track crankshaft angular speed and estimate engine combustion torque based on the experimental crankshaft angular speed of a four-cylinder Spark Ignition (SI) engine. Then, a new advance in the application of Artificial Neural Networks (ANNs) based on the estimated results of automated dynamic misfire fault diagnosis both under steady state and non-stationary condition is discussed in detailed. In order to effectively obtain data for network training, the estimated engine combustion torque is segmentally preprocessed according to the crank angle displacement of automobile engine. Furthermore, a series of experiments are carried out under normal and a variety of misfire conditions. The ANN systems are trained and tested using prepared cases. Finally, the Back-Propagation Neural Network (BPNN), Elman Neural Network (ENN), and Support Vector Machine (SVM) are applied to diagnose misfire fault, the effectiveness of each is evaluated respectively. Based on the estimated engine combustion torque, the experimental results show that the designed ENN is able to correctly diagnose misfire fault with a running time of 0.6 s, including single misfire, intermittent double-cylinder misfire, and continuous double-cylinder misfire in transient working condition.

# Summary. An optional shortened abstract.
summary: This work proposes a hybrid Luenberger–sliding mode state observer to estimate engine combustion torque, enabling effective ANN-based misfire fault diagnosis under both steady and transient conditions. Experimental results show that the Elman Neural Network achieves accurate and fast detection of diverse misfire scenarios.

tags:
- Fault Detection
featured: true

hugoblox:
  ids:
    # arxiv: 1512.04133v1
    doi: 10.1016/j.ymssp.2019.02.048

links:
  - type: pdf
    url: /publications/journal-article/journal-paper.pdf
  # - type: code
  #   url: https://github.com/HugoBlox/hugo-blox-builder
  # - type: dataset
  #   url: ""
  # - type: poster
  #   url: ""
  # - type: project
  #   url: ""
  # - type: slides
  #   url: https://www.slideshare.net/
  # - type: source
  #   url: ""
  # - type: video
  #   url: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  # caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/jdD8gXaTZsc)'
  focal_point: "center"
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

<!-- > [!NOTE]
> Click the *Cite* button above to demo the feature to enable visitors to import publication metadata into their reference management software. -->

<!-- > [!NOTE]
> Create your slides in Markdown - click the *Slides* button to check out the example. -->

<!-- Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
