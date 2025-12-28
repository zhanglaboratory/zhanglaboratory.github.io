---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  spacing: '6rem'

sections:
  # 1. 【改动】实验室欢迎头部 (替代原本的 Admin/Download CV)
  - block: markdown
    content:
      title: 'Welcome to Zhang Laboratory'
      subtitle: 'The Seventh Affiliated Hospital, Sun Yat-sen University'
      text: |
        Our laboratory integrates **clinical gastrointestinal surgery** with cutting-edge **translational research**. We bridge the gap between surgical oncology and basic science to identify novel therapeutic targets.
    design:
      columns: '1'
      background:
        gradient_mesh:
          enable: true

  # 2. 研究方向 (保持不变)
  - block: markdown
    content:
      title: '🔬 Research Focus'
      subtitle: ''
      text: |-
        **Key Research Areas:**
        
        1. **Clinical GI Oncology:** Minimally invasive surgical techniques (Robotic & Laparoscopic).
        2. **Non-coding RNA Genomics:** Investigating lncRNAs in tumor microenvironment.
        3. **Cardio-Oncology:** Mechanisms of Kinase Inhibitor-induced cardiotoxicity.
    design:
      columns: '1'

  # 3. 【新增】数据库板块 (展示 KICDB 和未来数据库)
  - block: markdown
    id: database  # <--- 对应导航栏的链接
    content:
      title: Databases & Tools
      subtitle: 'Open-source resources developed by our lab'
      text: |-
        ### 1. KICDB: A Causality-Oriented Multi-Omics Database for Kinase Inhibitor-Induced Cardiotoxicity
        
        [**👉 Click here to access KICDB**](https://zhang-lab-database.shinyapps.io/KICDB/)
        
        **Authors:** Jiamin Wei, Yin Liu, Miaoqing Wu, Guoyuan Li, Xinyao Zheng, Huafeng Fu, Jian Zhang, Jijin Lin
        
        **Abstract:**
        * **Background:** Kinase inhibitors (KIs) are mainstays of targeted cancer therapy, but their clinical utility is frequently limited by cardiotoxicity. A systematic resource to explore the underlying causal mechanisms is urgently needed.
        * **Methods:** We present the KICDB, a comprehensive and interactive web server built upon a framework integrating large-scale transcriptomics meta-analysis with causal inference.
        * **Results:** This database centralizes the findings from a comprehensive meta-analysis of 26 kinase inhibitors (KIs) across 7 studies (n=5291) identified 8,907 significant gene expression changes in human cardiomyocytes. To establish causality, we performed a two-pronged Mendelian randomization (MR) analysis. This large-scale analysis revealed 26 significant causal associations, implicating novel molecular mediators in KI-induced cardiotoxicity.
        * **Conclusions:** KICDB serves as a valuable and accessible platform for the cardio-oncology community.
        
        ---
        
        ### 2. Upcoming Database (Work in Progress)
        *More multi-omics databases for GI tumors are currently under development. Stay tuned.*
    design:
      columns: '1'

  # 4. 精选论文 (保持不变)
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

  # 5. 全部论文 (保持不变)
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

  # 6. 联系方式 (保持不变)
  - block: markdown
    id: contact
    content:
      title: Contact Us
      subtitle: ''
      text: |-
        To learn more about our research or potential collaborations, please reach out.
        
        **Email:** dr.jian.zhang.phd at gmail.com
        
        **Address:** The Seventh Affiliated Hospital, Sun Yat-sen University  
        Shenzhen, Guangdong, China 518107
    design:
      columns: '1'
      background:
        color: '#1a202c'
        text_color_light: true
---
