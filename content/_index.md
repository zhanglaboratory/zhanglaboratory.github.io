---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  spacing: '6rem'

sections:
  # 1. 个人简介 (保留)
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

  # 2. 研究介绍 (保留)
  - block: markdown
    content:
      title: '🔬 Research Focus'
      subtitle: ''
      text: |-
        Our laboratory integrates **clinical gastrointestinal surgery** with cutting-edge **translational research**.
        
        **Key Research Areas:**
        1. **Clinical GI Oncology:** Minimally invasive surgical techniques.
        2. **Non-coding RNA Genomics:** Investigating lncRNAs in tumor microenvironment.
        3. **Nanomedicine:** Targeted drug delivery systems.
    design:
      columns: '1'

  # 3. 精选论文 (保留)
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

  # 4. 全部论文 (修改：将 Papers 改为 Publications)
  - block: collection
    id: publications
    content:
      title: Recent Publications  # <--- 修改了这里
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation

  # (Talks, News, Projects, Courses 板块已被彻底删除)
---
