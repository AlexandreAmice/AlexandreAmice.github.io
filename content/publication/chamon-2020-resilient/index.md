---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Resilient control: Compromising to adapt'
subtitle: ''
summary: ''
authors:
- Luiz FO Chamon
- Alexandre Amice
- Santiago Paternain
- Alejandro Ribeiro
tags: []
categories: []
date: '2020-01-01'
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
projects: ["Constraint_Relax"]
publishDate: '2023-02-15T20:46:56.022741Z'
publication_types:
- '1'
abstract: — In optimal control problems, disturbances are typically dealt with using
  robust solutions, such as H∞ or tube model predictive control, that plan control
  actions feasible for the worst-case disturbance. Yet, planning for every contingency
  can lead to over-conservative, poorly performing solutions or even, in extreme cases,
  to infeasibility. Resilience addresses these shortcomings by adapting the underlying
  control problem, e.g., by relaxing its specifications, to obtain a feasible, possibly
  still valuable trajectory. Despite their different aspects, robustness and resilience
  are often conflated in the context of dynamical systems and control. The goal of
  this paper is to formalize, in the context of optimal control, the concept of resilience
  understood as above, i.e., in terms of adaptation. To do so, we introduce a resilient
  formulation of optimal control by allowing disruption-dependent modifications of
  the requirements that induce the desired resilient behavior. We then propose a framework
  to design these behaviors automatically by trading off control performance and requirement
  violations. We analyze this resilience-by-compromise method to obtain inverse optimality
  results and quantify the effect of disturbances on the induced requirement relaxations.
  By proving that robustness and resilience optimize different objectives, we show
  that these are in fact distinct system properties. We conclude by illustrating the
  effect of resilience in different control problems.
publication: '*IEEE* Conference on Decision and Control'
---
