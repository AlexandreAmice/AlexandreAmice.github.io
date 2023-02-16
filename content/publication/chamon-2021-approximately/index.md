---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Approximately supermodular scheduling subject to matroid constraints
subtitle: ''
summary: ''
authors:
- Luiz FO Chamon
- Alexandre Amice
- Alejandro Ribeiro
tags: []
categories: []
date: '2021-01-01'
lastmod: 2023-02-15T16:08:42-05:00
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
publishDate: '2023-02-15T21:08:41.791783Z'
publication_types:
- '2'
abstract: Control scheduling refers to the problem of assigning agents or actuators
  to act upon a dynamical system at specific times so as to minimize a quadratic control
  cost, such as the objective of the Linear-quadratic-Gaussian (LQG) or the Linear
  Quadratic Regulator (LQR). When budget or operational constraints are imposed on
  the schedule, this problem is in general NP-hard and its solution can therefore
  only be approximated even for moderately large systems. The quality of this approximation
  depends on the structure of both the constraints and the objective. This work shows
  that greedy scheduling is near-optimal when the constraints can be represented as
  an intersection of matroids, algebraic structures that encode requirements such
  as limits on the number of agents deployed per time slot, total number of actuator
  uses, and duty cycle restrictions. To do so, it proves that the LQG cost function
  is a-supermodular and provides a new a/(a + P )-optimality certificates for the
  greedy minimization of such functions over an intersections of P matroids. These
  certificates are shown to approach the 1/(1 + P ) guarantee of supermodular functions
  in relevant settings. These results support the use of greedy algorithms in non-supermodular
  quadratic control problems as opposed to typical heuristics such as convex relaxations
  and surrogate figures of merit, e.g., the log det of the controllability Gramian.
publication: '*IEEE Transactions on Automatic Control*'
---
