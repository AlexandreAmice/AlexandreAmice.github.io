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
    icon_pack: custom
    name: Interactive Python Notebooks
    url: https://deepnote.com/workspace/alexandre-amice-c018b305-0386-4703-9474-01b867e6efea/project/C-IRIS-7e82e4f5-f47a-475a-aad3-c88093ed36c6/notebook/2d_example_bilinear_alternation-14f1ee8c795e499ca7f577b6885c10e9
url_code: 'https://github.com/AlexandreAmice/drake/tree/C_Iris_Wafr_Journal_Examples/C_Iris_Examples'
url_pdf: ''
url_slides: ''
url_video: ''

bilbiography: references.bib

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# PDF: example
---
# Motivation

Understanding the geometry of collision-free configuration space (C-free) in the presence of task-space obstacles is an essential ingredient for collision-free motion planning.

Most work on the geometry of configuration space seeks to describe the configuration-space obstacle from the task-space description. This approach gives a "negative" description of C-free, describing it as the complement of this configuration space obstacle.

Nonetheless, many optimization-based motion planning frameworks can benefit greatly from a "positive" description of C-free, where in C-free is described as the union of simpler, often convex, sets. While it is possible to check for collisions at a point using standard algorithms, to date no practical method exists for computing C-free *regions* with rigorous certificates due to the complexity of mapping task-space obstacles through the kinematics. Therefore, the current literature provides no method for providing a positive description of C-free for these motion planning methods.

# Contribution
In this work, we provide a method for describing C-free using convex polyhedra in a bijective, rational parametrization of C-space known as the tangent configuration space (TC-space). Our primary technical contributions are two convex (specifically Sums-of-Squares (SOS)) programs which can certify that a polyhedron in TC-space contains no collision when the obstacles are specified as convex sets in *task space*. Similar to [(Deits et al. 2014)](https://groups.csail.mit.edu/robotics-center/public_papers/Deits14.pdf), we then construct certified, collision-free polytopic regions by alternating between a pair of convex programs. Our method works in arbitrary dimensions and is the first to our knowledge to provide rigorous certificates for non-zero volume sets in this setting. Moreover, we provide a fast, mature implementation of our technique in the open-source robotics toolbox [Drake](https://github.com/RobotLocomotion/drake).

# Results
We run our method on robots of varying complexity. Visit [this link](https://deepnote.com/workspace/alexandre-amice-c018b305-0386-4703-9474-01b867e6efea/project/C-IRIS-7e82e4f5-f47a-475a-aad3-c88093ed36c6/notebook/2d_example_bilinear_alternation-14f1ee8c795e499ca7f577b6885c10e9) to play with a variety of these examples yourself!

## A Two Dimensional Example
We consider a simple two degree of freedom robot where we can visualize both the task space on the left and the configuration space obstacle on the right. The green dot in the configuration space represents the current configuration. The red region corresponds to the configuration space obstacle, i.e. if the green dot wanders into the red region we have a collision. We animate a trajectory through our certified region and show the separating plane certificates for the tips of the two robots. The animation can be replayed by opening the control menu and hitting play on the animation (you may need to minimize the scene tab).
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

We also provide a visualization of our algorithm growing regions in this configuration space below.

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


## A Realistic Robot

Our work scales to various realistic robots. In this example, a collision-free configuration space region is grown near a pre-grasp pose for a UR3e to grip the red object. The animation shows the range of configurations which are certified as collision-free near the object.

<iframe 
  src="ur_single.html"
  width="100%"
  height="500"
  frameborder="1"
  allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
  allowfullscreen>
  name="pinball_trajectory"
</iframe>
<p><center><a href="ur_single.html" target="ur_single">View this animation in full screen</a></center></p>
