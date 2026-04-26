---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  # - block: resume-biography
  #   id: about
  #   content:
  #     # Choose a user profile to display (a folder name within `content/authors/`)
  #     username: admin
  #     # Override your bio text from `authors/admin/_index.md`?
  #     text:
  - block: resume-biography
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      # Override your bio text from `authors/admin/_index.md`?
      text:
      headings:
        about: ""
        education: ""
        interests: ""
      design:
        # Use the new Gradient Mesh which automatically adapts to the selected theme colors
        background:
          gradient_mesh:
            enable: true
            # Name heading sizing to accommodate long or short names
        name:
          size: xs # Options: xs, sm, md, lg (default), xl

        # Avatar customization
        avatar:
          size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
          shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: CV
      text: |-
        {{< button url="uploads/Amice_CV.pdf" icon="arrow-down-tray" align="center" >}}Download CV{{< /button >}}

  # Experience is set in me.yaml
  - block: resume-experience
    content:
      username: me
    design:
      # Education or Experience section first?
      is_education_first: false

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
      buttons:
        - name: All
          tag: "*"
        - name: Geometry of Configuration Space
          tag: Geometry
        - name: Optimization Software
          tag: "Optimization Software"
        - name: Constraint Relaxation
          tag: "Constraint_Relax"
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: "2"
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: true
---
