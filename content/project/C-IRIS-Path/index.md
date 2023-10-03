---
title: Certifying Trajectories in Seconds
summary: Formally verifying the safety of complicated trajectories at scale.
tags:
  - Geometry
date: '2023-10-02T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  focal_point: Smart
  caption: A pair of manipulators reach into a shelf. The red hyperplane certifies that the grippers do not collide at any point during the motion plan.

# links:
#   - icon: deepnote
#     icon_pack: custom
#     name: Interactive Python Notebooks
#     url: https://deepnote.com/workspace/alexandre-amice-c018b305-0386-4703-9474-01b867e6efea/project/C-IRIS-7e82e4f5-f47a-475a-aad3-c88093ed36c6/notebook/2d_example_bilinear_alternation-14f1ee8c795e499ca7f577b6885c10e9
# url_code: 'https://github.com/AlexandreAmice/drake/tree/C_Iris_Wafr_Journal_Examples/C_Iris_Examples'
# url_pdf: ''
# url_slides: ''
# url_video: ''

bilbiography: references.bib

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# PDF: example
---
# THIS PAGE IS UNDER CONSTRUCTION
# Video Summary
<video width="320" height="240" controls>
  <source src="IcraFinalVideo.mp4" type="video/mp4">
</video>

# Motivation

Collision-free motion planning is a fundamental problem in the safe and efficient operation of any robotic system. One of the most important subroutines in collision-free motion planning is collision detection, which has been studied extensively. Algorithms for checking whether a single configuration is collision free are quite mature and can be performed in microseconds on modern hardware.

By contrast, algorithms which are capable of certifying non-collision for the infinite family of configurations along a motion plan are less common. Known as dynamic collision checking, this subroutine is performed hundreds to thousands of times in randomized motion planning methods, and so the speed as well as the correctness of these algorithms is central to their adoption. Due to the speed requirement, it is common practice to heuristically perform dynamic collision checking by sampling a finite number of static configurations along the motion plan. Nevertheless, it is widely recognized that this is insufficient for safety critical robots.

Current methods for formally checking the safety of robots frequently only apply to piecewise linear motion plans and are either too slow for practical deployment, rely on difficult to acquire parameters, or are too conservative for certifying motion plans in tight spaces.
<!-- put the video of the two iiwas with different levels of safety -->


# Contribution
In this work, we provide a method for certifying that a robot trajectory contains no collisions. The method provides rigorous proofs of non-collision using Sums-of-Squares optimization, can certify piecewise-polyonmial paths of arbitrary degree, and is efficient enough to certify the safety of a bimanual manipulator motion plan in just over a second. Moreover, it is efficient enough to discriminate the safety of two motion plans which differ by only millimeters.


# Visualizing the Certificates
The certificates of non-collision can be visualized as hyperplanes in the task space. Click "Open Controls" to turn different hyperplanes on and off, replay the animation, and more.
<iframe 
  width="100%"
  height="500"
  src="14dof_hyperplanes.html"
  frameborder="1"
  allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
  allowfullscreen>
  name="14dof_hyperplanes"
</iframe>
<p><center><a href="14dof_hyperplanes.html" target="14dof_hyperplanes">View and interact with this animation in full screen</a></center></p>
