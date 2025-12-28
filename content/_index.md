---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  spacing: '6rem'

sections:
  # 1. Biography (个人简介)
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

  # 2. Research Focus (研究方向)
  - block: markdown
    content:
      title: '🔬 Research Focus'
      subtitle: ''
      text: |-
        Our laboratory is dedicated to **Precision Medicine** in Gastrointestinal Oncology. 
        
        We combine **surgical expertise** with **multi-omics analysis** to identify novel therapeutic targets. Our current flagship project includes the **Kinase Inhibitor Cardiotoxicity Database (KICDB)**.
    design:
      columns: '1'

  # 3. Featured Publications (精选论文)
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

  # 4. Recent Publications (全部论文)
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

  # 5. Contact / Footer (新增的底部联系方式，仿 Han Lab 风格)
  - block: contact
    id: contact
    content:
      title: Contact Us
      subtitle: ''
      text: 'To learn more about our research or potential collaborations, please reach out.'
      email: dr.jian.zhang.phd@gmail.com
      address:
        street: 'The Seventh Affiliated Hospital, Sun Yat-sen University'
        city: 'Shenzhen'
        region: 'China'
        postcode: '518107'
        country: 'China'
        country_code: 'CN'
    design:
      columns: '2'
      background:
        text_color_light: true # 强制文字变白
        color: '#1a202c' # 深黑色背景 (类似 Han Lab)
---
