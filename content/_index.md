---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  spacing: '6rem'

sections:
  # 1. 实验室欢迎语 (使用 Markdown 表格布局，稳如泰山)
  - block: markdown
    content:
      title: ''
      subtitle: ''
      text: |
        | | |
        | :--- | :--- |
        | <img src="uploads/cartoon.jpg" width="800px" style="border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);"> | <h1>Welcome to Zhang Laboratory</h1><br>**The Seventh Affiliated Hospital, Sun Yat-sen University**<br><br>Our laboratory represents a unique convergence of **high-volume clinical surgery** and **advanced translational science**.<br><br>Led by **Dr. Jian Zhang**, an Associate Chief Physician **specializing in the treatment of gastrointestinal tumors**, our team is dedicated to solving clinical challenges through multi-omics discovery and nanomedicine innovation. |
    design:
      columns: '1'
      background:
        gradient_mesh:
          enable: true

  # 2. 研究方向
  - block: markdown
    content:
      title: '🔬 Research Focus'
      subtitle: ''
      text: |-
        Our research is supported by the **National Natural Science Foundation of China (NSFC)** and focuses on three strategic pillars:
        
        ### 1. Precision GI Oncology & Surgery
        * **Minimally Invasive Surgery:** Optimizing robotic and laparoscopic techniques for gastric and colorectal cancer.
        * **Clinical Translation:** Improving patient outcomes through biomarker-guided surgical strategies.
        
        ### 2. Non-coding RNA & Epigenetics
        * **Mechanistic Study:** Investigating the roles of **lncRNAs** (e.g., *GHRLOS*, *FAL1*) and **alternative splicing** in tumor metastasis and chemoresistance.
                
        ### 3. Nanomedicine & Drug Delivery
        * **Targeted Therapy:** Developing **biomimetic nanoparticles** for precise drug delivery.
        * **Cardio-Oncology:** utilizing the **KICDB** database to mitigate kinase inhibitor-induced cardiotoxicity.
    design:
      columns: '1'

  # 3. 数据库板块
  - block: markdown
    id: database
    content:
      title: Databases & Tools
      subtitle: 'Open-source resources developed by our lab'
      text: |-
        ### 1. KICDB: A Causality-Oriented Multi-Omics Database for Kinase Inhibitor-Induced Cardiotoxicity
        
        [**👉 Click here to access KICDB**](https://zhang-lab-database.shinyapps.io/KICDB/)
        
        **Overview:** KICDB integrates large-scale transcriptomics meta-analysis (n=5291) with Mendelian randomization to identify causal mechanisms of cardiotoxicity induced by 26 kinase inhibitors.
    design:
      columns: '1'

  # 4. 精选论文
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: card
      columns: 2

  # 5. 全部论文
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

  # 6. 联系方式
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
