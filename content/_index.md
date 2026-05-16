---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
      spacing:
        padding: [1rem, 1rem, 1rem, 1rem]
  - block: markdown
    content:
      title: '🔬 My Research Interests'
      subtitle: ''
      text: |-
        My research interests sit at the intersection of **semi-supervised learning**, **graph representation learning**, **computer vision**, **natural language processing**, and **large language models**, with a growing interest in **multi-agentic systems** and how heterogeneous models can collaboratively learn from one another under label scarcity.

        I am drawn to problems where data is messy, partially labelled, or distributed across modalities — exactly the conditions found in real-world healthcare, finance, and safety-critical applications. My goal is to design rigorous, reproducible, publication-quality methods that work in the real world.

        I am currently building **CLADBench**, an open-source, publication-grade benchmark for Collaborative Learning in Graph Anomaly Detection, as my M2 thesis at the LIRIS laboratory.
    design:
      columns: '1'
  - block: markdown
    id: papers
    content:
      title: Featured Publications
      text: |-
        [![Driver Safety using Human Pose Estimation](/uploads/featured-publication.png)](/publication/driver-safety-icet/)

        **Computer Vision**

        ### [Driver Safety using Human Pose Estimation](/publication/driver-safety-icet/)

        A YOLOv8-based real-time pose estimation pipeline with attention over safety-critical regions for driver fatigue and drowsiness classification on the DriPE dataset.

        [Read publication](/publication/driver-safety-icet/)
    design:
      columns: '1'
  - block: collection
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: projects
    content:
      title: Selected Projects
      text: ''
      filters:
        folders:
          - projects
        exclude_featured: false
      count: 6
    design:
      view: article-grid
      columns: 3
      spacing:
        padding: [1rem, 1rem, 1rem, 1rem]
---
