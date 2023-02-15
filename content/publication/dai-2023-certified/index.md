---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Certified Polyhedral Decompositions of Collision-Free Configuration Space
subtitle: ''
summary: ''
authors:
- Hongkai Dai*
- Alexandre Amice*
- Peter Werner
- Annan Zhang
- Russ Tedrake
tags: []
categories: []
date: '2023-01-01'
lastmod: 2023-02-15T15:44:48-05:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: ["C-IRIS"]
publishDate: '2023-02-15T20:44:48.538760Z'
publication_types:
- '3'
abstract: Understanding the geometry of collision-free configuration space (C-free)
  in the presence of task-space obstacles is an essential ingredient for collision-free
  motion planning. While it is possible to check for collisions at a point using standard
  algorithms, to date no practical method exists for computing C-free regions with
  rigorous certificates due to the complexity of mapping task-space obstacles through
  the kinematics. In this work, we present the first to our knowledge rigorous method
  for approximately decomposing a rational parametrization of C-free into certified
  polyhedral regions. Our method, called C-IRIS (C-space Iterative Regional Inflation
  by Semidefinite programming), generates large, convex polytopes in a rational parameterization
  of the configuration space which are rigorously certified to be collision-free.
  Such regions have been shown to be useful for both optimization-based and randomized
  motion planning. Based on convex optimization, our method works in arbitrary dimensions,
  only makes assumptions about the convexity of the obstacles in the task space, and
  is fast enough to scale to realistic problems in manipulation. We demonstrate our
  algorithm's ability to fill a non-trivial amount of collision-free C-space in several
  2-DOF examples where the C-space can be visualized, as well as the scalability of
  our algorithm on a 7-DOF KUKA iiwa, a 6-DOF UR3e and 12-DOF bimanual manipulators.
  An implementation of our algorithm is open-sourced in Drake.
publication: ''
---
