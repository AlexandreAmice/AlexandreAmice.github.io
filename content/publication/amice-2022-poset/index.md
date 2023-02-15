---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Solving Least Squares Problems on Partially Ordered Sets
subtitle: ''
summary: ''
authors:
- Alexandre Amice
- Pablo Parrilo
tags: []
categories: []
date: '2022-01-01'
lastmod: 2023-02-15T15:46:57-05:00
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
projects: ["Poset_Least_Squares"]
publishDate: '2023-02-15T20:46:56.835078Z'
publication_types:
- '1'
abstract: We study a general class of least-squares problems structured according
  to a partially ordered set (poset). This is a fundamental optimization problem underlying
  the design of structured controllers on directed acyclic graphs or posets. We show
  that the optimality conditions of this problem yield a structured linear system,
  with sparsity pattern determined by a derived poset known as the poset of intervals.
  In general, this system could be relatively dense, and thus standard sparse linear
  algebra techniques may fail to provide significant reduction in computational complexity.
  Nonetheless, for a broad class of posets called multitrees identified in (Nayyar
  2015) we show that performing elimination according to an order defined by the poset
  intervals progressively decouples variables, reducing the arithmetic complexity
  of solving the problem.
publication: '*IEEE* Conference on Decision and Control'
---
