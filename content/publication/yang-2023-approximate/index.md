---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Approximate Optimal Controller Synthesis for Cart-Poles and Quadrotors via Sums-of-Squares
subtitle: ''
summary: ''
authors:
- Lujie Yang
- Hongkai Dai
- Alexandre Amice
- Russ Tedrake
tags: []
categories: []
date: '2023-09-01'
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
- '2'
abstract: Sums-of-squares (SOS) optimization is a promising tool to synthesize certifiable controllers for nonlinear dynamical systems. Building upon prior works, we demonstrate that SOS can synthesize dynamic controllers with bounded suboptimal performance for various underactuated robotic systems by finding good approximations of the value function. We summarize a unified SOS framework to synthesize both under- and over- approximations of the value function for continuous-time, control-affine systems, use these approximations to generate approximate optimal controllers, and perform regional analysis on the closed-loop system driven by these controllers. We then extend the formulation to handle hybrid systems with contacts. We demonstrate that our method can generate tight under- and over- approximations of the value function with low-degree polynomials, which are used to provide stabilizing controllers for continuoustime systems including the inverted pendulum, the cart-pole, and the quadrotor as well as a hybrid system, the planar pusher. To the best of our knowledge, this is the first time that a SOS-based time-invariant controller can swing up and stabilize a cart-pole, and push the planar slider to the desired pose. Videos at https://youtu.be/QQRpPNPeyg; demo code at https://deepnote.com/workspace/lujieyang/project/hjb-sos.
publication: ''
---
