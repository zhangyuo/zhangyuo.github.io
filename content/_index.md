---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Curriculum Vitae
        url: https://docs.google.com/document/d/e/2PACX-1vRURV0OdD3xCG4ABZqObpPUgqGH-u46rvePJIZ6nlZSgvjPeak16G01vVm35n9K-A/pub

      headings:
        about: 'Biography'
        education: ''
        interests: ''
    design:
      # Apply a gradient background
      css_class: hbx-bg-gradient
      # css_class: 'max-w-4xl mx-auto'
      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
      spacing:
        padding: [0, 0, 0, 0]
      # background:
      #   image:
      #     filename: stacked-peaks.svg
      #   position: center
      #   size: cover
      #   parallax: true
      #   text_color_light: true

  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        My research lies at the intersection of **graph neural networks (GNNs)**, **explainable AI**, and **secure machine learning**.  
        
        Recently, I developed a unified framework that bridges **adversarial attacks** and **counterfactual explanations**, enabling more faithful, concise, and plausible interpretations of GNN predictions.

        Looking ahead, my PhD research will explore **graph data watermarking** and **LLM-GraphRAG**, aiming to design **radio-active datasets** that embed detectable watermarks. This work links to **data poisoning, robustness, and trustworthy AI**, while offering practical tools for **intellectual property protection** in machine learning.  

        More broadly, I am excited about bridging **explainability, security, and foundation models**, and I actively welcome collaborations on **GNN explainability**, **watermarking across modalities**, and **LLM-based graph reasoning**.
    design:
      columns: '1'
      css_class: max-w-3xl mx-auto

  - block: collection
    id: papers
    content:
      title: '⭐ Featured Publications'
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection
    content:
      title: '📑 Recent Publications'
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
  
  - block: collection
    id: news
    content:
      title: '📣 Recent News'
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: news
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: card
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]

  - block: collection
    id: talks
    content:
      title: '🗣️ Recent & Upcoming Talks'
      filters:
        folders:
          - talks
    design:
      view: card

  - block: collection
    id: courses
    content:
      title: '🏫 Courses'
      subtitle: ''
      text: ''
      filters:
        folders:
          - courses
    design:
      view: card
  
  # 💼 工作经历
  - block: resume-experience
    id: experience
    content:
      title: '💼 Experiences'
      username: admin
    design:
      date_format: 'Jan 2006'

  # 🛠 技能
  - block: resume-skills
    id: skills
    content:
      title: '🛠 Skills'
      username: admin
    design:
      show_skill_percentage: true

  # 🏆 奖项
  - block: resume-awards
    id: awards
    content:
      title: '🏆 Awards'
      username: admin

  # 🌍 语言
  - block: resume-languages
    id: languages
    content:
      title: '🌍 Languages'
      username: admin
  
  - block: collection
    id: projects
    content:
      title: '🚀 Projects'
      filters:
        folders:
          - projects
        featured_only: false
    design:
      view: article-grid
      columns: 3

  - block: markdown
    id: contact
    content:
      title: '📬 Contact Me'
      subtitle: ''
      text: |-
        Feel free to reach out via email or social media:

        - **Email:** [yuzhang@cs.aau.dk](mailto:yuzhang@cs.aau.dk)  
        - **GitHub:** [github.com/zhangyuo](https://github.com/zhangyuo)  
        - **LinkedIn:** [Yu Zhang](http://www.linkedin.com/in/yu-zhang-580858167/)  
    design:
      columns: '1'

  # - block: cta-card
  #   demo: true # Only display this section in the Hugo Blox Builder demo site
  #   content:
  #     title: 👉 Build your own academic website like this
  #     text: |-
  #       This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

  #       <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

  #       Easily build anything with blocks - no-code required!

  #       From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
  #     button:
  #       text: Get Started
  #       url: https://hugoblox.com/templates/
  #   design:
  #     card:
  #       # Card background color (CSS class)
  #       css_class: 'bg-primary-300'
  #       css_style: ''
---
