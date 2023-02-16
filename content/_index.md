---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  # - block: about.avatar
  #   id: about
  #   content:
  #     # Choose a user profile to display (a folder name within `content/authors/`)
  #     username: admin
  #     # Override your bio text from `authors/admin/_index.md`?
  #     text:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:

  # - block: features
  #   content:
  #     title: Skills
  #     items:
  #       - name: R
  #         description: 90%
  #         icon: r-project
  #         icon_pack: fab
  #       - name: Statistics
  #         description: 100%
  #         icon: chart-line
  #         icon_pack: fas
  #       - name: Photography
  #         description: 10%
  #         icon: camera-retro
  #         icon_pack: fas
  - block: portfolio
    id: projects
    
    content:
      title: Research Projects
      subtitle: 
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      # buttons:
      #   - name: All
      #     tag: '*'
      #   - name: Geometry of Configuration Space
      #     tag: Geometry
      #   - name: Constraint Relaxation
      #     tag: 
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: true
  # - block: markdown
  #   content:
  #     title: Gallery
  #     subtitle: ''
  #     text: |-
  #       {{< gallery album="demo" >}}
  #   design:
  #     columns: '1'
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Doctoral Student 
          company: MIT
          company_url: ''
          company_logo: mit_logo
          location: Cambridge, MA
          date_start: '2020-08-01'
          date_end: ''
          description: Research in optimization methods for the control and verification of complex dynamical. systems.

        - title: Open Source Developer
          company: Drake Robotics Project
          company_url: drake.mit.edu
          company_logo: drake-dragon
          location: ''
          date_start: '2022-01-01'
          date_end: ''
          description: Contributions to symbolic algebra and mathematical optimization packages.

        - title: Masters and Undergraduate Researcher
          company: University of Pennsylvania
          company_url: ''
          company_logo: penn-logo
          location: Philadelphia, PA
          date_start: '2018-01-01'
          date_end: '2020-08-01'
          description: Research in discrete and convex optimization for resilient control systems.
          
        - title: Robotic Perception Intern
          company: Uber Advanced Technology Group
          company_url: ''
          company_logo: uber
          location: Pittsburgh, PA
          date_start: '2019-05-31'
          date_end: '2019-08-20'
          description: Research and development of radar perception systems.

    design:
      columns: '2'

  - block: markdown
    content:
      title: CV
      subtitle: "[View my full CV](uploads/Amice_CV.pdf)"
      text: 
      
  
  - block: collection
    content:
      title: Recent Publications
      filters:
        folders:
          - publication
        exclude_featured: False

  - block: markdown
    content:
      title: Contact Me
      subtitle: "[amice@mit.edu](mailto:amice@mit.edu)"

---


