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
      # IMPORTANT: Changed 'me' to 'admin' to match your folder content/authors/admin/
      username: admin
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: 'About Me'
        education: 'Education'
        interests: 'Interests'
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md

      # Avatar customization
      avatar:
        size: medium
        shape: circle

  - block: markdown
    content:
      title: '🔬 Research Focus'
      subtitle: ''
      text: |-
        Our laboratory integrates **clinical gastrointestinal surgery** with cutting-edge **translational research**. Based at the Seventh Affiliated Hospital of Sun Yat-sen University, we bridge the gap between surgical oncology and basic science.
        
        **Key Research Areas:**
        
        1. **Clinical GI Oncology:** Minimally invasive surgical techniques (Robotic & Laparoscopic) for gastric and colorectal cancer.
        2. **Non-coding RNA Genomics:** Investigating the role of lncRNAs (e.g., *GHRLOS*, *FAL1*) in tumor microenvironment and chemoresistance.
        3. **Nanomedicine:** Development of biomimetic nanoparticles and targeted drug delivery systems.

        We also maintain the **Kinase Inhibitor Cardiotoxicity Database (KICDB)**.
        
        Please reach out to collaborate 😃
    design:
      columns: '1'

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
