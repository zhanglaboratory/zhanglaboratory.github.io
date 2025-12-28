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

# 5. Contact (替代方案：使用 markdown 手写联系方式)
  - block: markdown
    id: contact
    content:
      title: Contact Us
      subtitle: ''
      text: |-
        To learn more about our research or potential collaborations, please reach out.
        
        **Email:** dr.jian.zhang.phd@gmail.com
        
        **Address:** The Seventh Affiliated Hospital, Sun Yat-sen University  
        Shenzhen, Guangdong, China 518107
    design:
      columns: '1'
      background:
        color: '#1a202c' # 深黑色背景
        text_color_light: true # 文字强制变白
