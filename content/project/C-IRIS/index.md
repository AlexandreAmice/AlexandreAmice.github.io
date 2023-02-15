---
title: Certified Polyhedral Descriptions of Configuration Space
summary: Provable correct descriptions of Configuration Space for collision-free motion planning
tags:
  - Geometry
date: '2023-02-12T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  focal_point: Smart

links:
  - icon: deepnote
    icon_pack: fab
    name: Interactive Python Notebooks
    url: https://deepnote.com
url_code: 'https://github.com/AlexandreAmice/drake/tree/C_Iris_Wafr_Journal_Examples'
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# PDF: example
---


Understanding the geometry of collision-free configuration space (C-free) in the presence of task-space obstacles is an essential ingredient for collision-free motion planning. While it is possible to check for collisions at a point using standard algorithms, to date no practical method exists for computing C-free *regions* with rigorous certificates due to the complexity of mapping task-space obstacles through the kinematics. In this work, we present the first to our knowledge rigorous method for approximately decomposing a rational parametrization of C-free into certified polyhedral regions. Our method, called C-IRIS (C-space Iterative Regional Inflation by Semidefinite programming), generates large, convex polytopes in a rational parameterization of the configuration space which are rigorously certified to be collision-free. Such regions have been shown to be useful for both optimization-based and randomized motion planning. Based on convex optimization, our method works in arbitrary dimensions, only makes assumptions about the convexity of the obstacles in the *task* space, and is fast enough to scale to realistic problems in manipulation. We demonstrate our algorithm's ability to fill a non-trivial amount of collision-free C-space in several 2-DOF examples where the C-space can be visualized, as well as the scalability of our algorithm on a 7-DOF KUKA iiwa, a 6-DOF UR3e and 12-DOF bimanual manipulators. An implementation of our algorithm is open-sourced in [Drake](https://github.com/RobotLocomotion/drake).




<iframe 
  src="pinball_growth.html"
  width="100%"
  height="500"
  frameborder="1"
  allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
  allowfullscreen>
  name="pinball_trajectory"
</iframe>
<p><center><a href="pinball_growth.html" target="pinball_growth">View this animation in full screen</a></center></p>

<iframe 
  width="100%"
  height="500"
  src="pinball_trajectory.html"
  frameborder="1"
  allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
  allowfullscreen>
  name="pinball_trajectory"
</iframe>
<p><center><a href="pinball_trajectory.html" target="pinball_trajectory">View this animation in full screen</a></center></p>


