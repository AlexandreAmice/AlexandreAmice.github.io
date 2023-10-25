---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Approximating Robot Configuration Spaces with few Convex Sets using Clique Covers of Visibility Graphs
subtitle: ''
summary: ''
authors:
- Peter Werner
- Alexandre Amice
- Tobia Marcucci
- Daniela Rus
- Russ Tedrake
tags: []
categories: []
date: '2023-10-09'
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
publication_types:
- '3'
abstract: Many computations in robotics can be dramatically accelerated if the robot configuration space is described as a collection of simple sets. For example, recently developed motion planners rely on a convex decomposition of the free space to design collision-free trajectories using fast convex optimization. In this work, we present an efficient method for approximately covering complex configuration spaces with a small number of polytopes. The approach constructs a visibility graph using sampling and generates a clique cover of this graph to find clusters of samples that have mutual line of sight. These clusters are then inflated into large, full-dimensional, polytopes. We evaluate our method on a variety of robotic systems and show that it consistently covers larger portions of free configuration space, with fewer polytopes, and in a fraction of the time compared to previous methods.
publication: ''
---
