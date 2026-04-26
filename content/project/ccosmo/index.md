---
title: "CCosmo: A Custom First-Order Conic Solver"
summary: A C++ and CUDA solver family for the structured convex programs that appear in robotics, control, and graph-of-convex-sets relaxations.
tags:
  - Optimization Software
  - Conic Optimization
  - Robotics
date: "2026-04-26T00:00:00Z"

external_link: ""

image:
  focal_point: Smart
  caption: CCosmo is a custom conic solver family built around structure-aware linear algebra and batch solves.

# links:
#   - type: code
#     url: "https://github.com/AlexandreAmice/gcs_solver"
url_pdf: ""
url_slides: ""
url_video: ""
---

# Motivation

Convex optimization appears throughout robotics, but in markedly different forms: small, dense quadratic programs (QPs) arise in online whole-body control, inverse-kinematics controllers, and reduced-order MPC controllers; moderately sized, sparse and dense quadratic and second-order cone programs (SOCPs) arise naturally in grasp selection and contact planning problems due to friction constraints; large, structured, and sparse problems arise in the context of trajectory optimization, with complicated semidefinite constraints becoming increasingly popular in the localization, perception, and motion planning communities.

In many of these applications, solvers are part of a larger planning, control, or estimation loop that repeatedly solve closely related problems to moderate accuracy at high speeds.
This setting favors first-order methods, which have low memory requirements, are naturally warm started, and often converge rapidly to the accuracy required in the outer loop.
Moreover, the relative simplicity of first-order methods makes them easy to customize to different classes of instances, sizes, and hardware such as massive programs on compute clusters, tiny programs on embedded hardware, or batches of programs on GPUs.

# Contribution

`CCosmo` is a C++ implementation of a first-order conic optimization method designed to be customized around the problem family being solved. The core solver handles convex programs with quadratic costs.
`CCosmo` is based on the same algorithm as the popular [`OSQP`](https://osqp.org/) and [`COSMO.jl`](https://oxfordcontrol.github.io/COSMO.jl/stable/) solvers from the Oxford Control Group.

In addition to the usual quadratic-cost, convex standard form program, `CCosmo` supports programs in a matrix-standard-form that commonly arises when solving convex relaxations of non-convex programs. This is enabled by a custom matrix-linear-algebra backend.
Finally, `CCosmo` also includes a GPU backend for solving large batches of very small programs.

# Results

PENDING CODE RELEASE

# Code

`CCosmo` will be released publicly soon!
