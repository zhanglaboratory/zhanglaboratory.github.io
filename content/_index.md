---
title: ''
date: 2022-10-24
type: landing

design:
  spacing: '6rem'

sections:
  # 1. Biography (读取刚才修改的 admin 信息)
  - block: resume-biography-3
    content:
      username: admin
      text: ''
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      background:
        gradient_mesh:
          enable: true
      avatar:
        size: medium
        shape: circle

  # 2. Research Focus
  - block: markdown
    content:
      title: '🔬 Research Focus'
      subtitle: ''
      text: |-
        Our laboratory is dedicated to **Precision Medicine** in Gastrointestinal Oncology. 
        
        We combine **surgical expertise** with **multi-omics analysis** to identify novel therapeutic targets. Our current flagship project includes the **Kinase Inhibitor Cardiotoxicity Database (KICDB)**.
    design:
      columns: '1'

  # 3. Featured Publications
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2

  # 4. Recent Publications
  - block: collection
    id: publications
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
---
