---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Discrete Approximate Information States in Partially Observable Environments
subtitle: ''
summary: ''
authors:
- Lujie Yang
- Kaiqing Zhang
- Alexandre Amice
- Yunzhu Li
- Russ Tedrake
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
projects: []
publishDate: '2023-02-15T20:46:57.132490Z'
publication_types:
- '1'
abstract: The notion of approximate information states (AIS) was introduced in (Subramanian
  2020) as a methodology for learning task-relevant state representations for control
  in partially observable systems. They proposed particular learning objectives which
  attempt to reconstruct the cost and next state and provide a bound on the suboptimality
  of the closed-loop performance, but it is unclear whether these bounds are tight
  or actually lead to good performance in practice.  Here we study this methodology
  by examining the special case of discrete approximate information states (DAIS).
  In this setting, we can solve for the globally optimal policy using value iteration
  for the DAIS model, allowing us to disambiguate the performance of the AIS objective
  from the policy search. Going further, for small problems with finite information
  states, we reformulate the DAIS learning problem as a novel mixed-integer program
  (MIP) and solve it to its global optimum; in the infinite information states case,
  we introduce clustering-based and end-to-end gradient-based optimization methods
  for minimizing the DAIS construction loss. We study DAIS in three partially observable
  environments and find that the AIS objective offers relatively loose bounds for
  guaranteeing monotonic performance improvement and is sufficient but not necessary
  for implementing optimal controllers. DAIS may even prove useful in practice by
  itself or as part of mixed discrete- and continuous-state representations, due to
  its ability to represent logical state, to its potential interpretabilty, and to
  the availability of these stronger algorithms.
publication: ''
---
