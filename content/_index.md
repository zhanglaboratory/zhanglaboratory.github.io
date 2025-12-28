---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  spacing: '4rem'

sections:
  # 1. 实验室欢迎语 (文字部分)
  - block: markdown
    content:
      title: 'Welcome to Zhang Laboratory'
      subtitle: 'The Seventh Affiliated Hospital, Sun Yat-sen University'
      text: |
        Our laboratory represents a unique convergence of **high-volume clinical surgery** and **advanced translational science**.
        
        Led by **Dr. Jian Zhang**, an Associate Chief Physician **specializing in the treatment of gastrointestinal tumors**, our team is dedicated to solving clinical challenges through multi-omics discovery and nanomedicine innovation.
    design:
      columns: '1'
      background:
        gradient_mesh:
          enable: true

  # 2. 底部卡通图片 (已修复路径)
  - block: markdown
    content:
      title: ''
      subtitle: ''
      text: |
        <div style="text-align: center;">
          <img src="/uploads/cartoon.jpg" alt="Zhang Lab Team" style="width: 90%; max-width: 600px; border-radius: 15px; box-shadow: 0 5px 15px rgba(0,0,0,0.1);">
        </div>
    design:
      columns: '1'
---
