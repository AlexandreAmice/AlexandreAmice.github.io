---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Matroid-constrained approximately supermodular optimization for near-optimal
  actuator scheduling
subtitle: ''
summary: ''
authors:
- Luiz FO Chamon
- Alexandre Amice
- Alejandro Ribeiro
tags: []
categories: []
date: '2019-01-01'
lastmod: 2023-02-15T15:46:56-05:00
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
projects: ["Matroid"]
publishDate: '2023-02-15T20:46:56.285778Z'
publication_types:
- '1'
abstract: 'This work considers the problem of scheduling actuators to minimize the
  Linear Quadratic Regulator (LQR) objective. In general, this problem is NP-hard
  and its solution can therefore only be approximated even for moderately large systems.
  Although convex relaxations have been used to obtain these approximations, they
  do not come with performance guarantees. Another common approach is to use greedy
  search. Still, classical guarantees do not hold for the scheduling problem because
  the LQR cost function is neither submodular nor supermodular. Though surrogate supermodular
  figures of merit, such as the log det of the controllability Gramian, are often
  used as a workaround, the resulting problem is not equivalent to the original LQR
  one. This work shows that no change to the original problem is needed to obtain
  performance guarantees. Specifically, it proves that the LQR cost function is approximately
  supermodular and provides new near-optimality certificates for the greedy minimization
  of these functions over a generic matroid. These certificates are shown to approach
  the classical 1/2 guarantee of supermodular functions in relevant application scenarios. '
publication: '*IEEE* Conference on Decision and Control'
---
