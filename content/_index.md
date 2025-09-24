---
# Leave the homepage title empty to use the site title
title: ""
date: 2024-05-21
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: My CV
        url: uploads/Wang_Haocheng_CV.pdf 
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  
  - block: markdown
    id: research
    content:
      title: '🧠 Research'
      subtitle: ''
      text: |-
        My research focuses on enhancing large language models' capabilities in formal mathematical reasoning and automated theorem proving. I'm particularly interested in:

        - **Formal Theorem Proving**: Developing techniques to formalize mathematical theorems and proofs using tools like Lean 4
        - **LLMs for Mathematical Reasoning**: Training and fine-tuning large language models to improve mathematical reasoning capabilities
        - **Agent Building**: Creating intelligent agents that can autonomously tackle complex mathematical problems
        - **Reinforcement Learning**: Applying RL techniques to improve LLM performance on theorem proving tasks

        I apply a range of quantitative methods and deep learning approaches to build systems that can advance the state of artificial mathematical reasoning.
        
        Please reach out if you're interested in collaborating! 📧
    design:
      columns: '1'
  
  - block: collection
    id: publications
    content:
      title: Featured Research Papers
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: citation
      columns: 1

  - block: markdown
    content:
      title: 'Research Projects'
      subtitle: ''
      text: |-
        ### DeepSeek-Prover-V1.5 & V2
        Developed a novel hybrid approach combining LLMs and Monte-Carlo tree search for automated theorem proving. Our approach achieved state-of-the-art results on the miniF2F (63.5%) and ProofNet (25.3%) benchmarks.

        ### LeanBENCH
        Currently developing a comprehensive benchmark for autoformalization of college-level and olympiad-level mathematics in Lean4. This ongoing project aims to create a dataset of 12k formalized mathematical problems.

        ### Formalization of Auction Theory
        Working on formalizing auction theory in game theory using Lean4, including second price auction DSIC and Myerson's lemma. Contributing to the GameTheory repository and Mathlib4.
    design:
      columns: '1'

  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      view: compact
      columns: 2

  - block: markdown
    content:
      title: 'Awards & Recognition'
      subtitle: ''
      text: |-
        - **Intel Young Talent Award**, 34th China Adolescents Science & Technology Innovation Contest (2019)
        - **Students' Projects Third Award**, 34th China Adolescents Science & Technology Innovation Contest (2019)
        - **The First Place Award**, 33rd Henan Province Science and Technology Innovation Competition (2019)
        - **The First Place of Grand Award**, 3rd International Youth Science Fair for Discovery Videos (2018)
    design:
      columns: '1'
---