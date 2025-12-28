---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  spacing: '4rem'

sections:
  # 1. 实验室欢迎语 (清理了手动字号，自动继承全局 CSS)
  - block: markdown
    content:
      title: ''
      subtitle: ''
      text: |
        <div style="text-align: center; max-width: 900px; margin: 0 auto;">
          <h1>Welcome to Zhang Laboratory</h1>
          
          <p style="font-weight: bold; color: #666;">
            The Seventh Affiliated Hospital, Sun Yat-sen University
          </p>
          
          <p>
            Our laboratory represents a unique convergence of <strong>high-volume clinical surgery</strong> and <strong>advanced translational science</strong>.
          </p>
          
          <p>
            Led by <strong>Dr. Jian Zhang</strong>, an Associate Chief Physician <strong>specializing in the treatment of gastrointestinal tumors</strong>, our team is dedicated to solving clinical challenges through multi-omics discovery and nanomedicine innovation.
          </p>
        </div>
    design:
      columns: '1'
      background:
        gradient_mesh:
          enable: true

  # 2. 底部卡通图片
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
