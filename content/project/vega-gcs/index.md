---
title: "VEGA: Decomposition Solver for Graphs of Convex Sets"
summary: Parallel decomposition methods and benchmark infrastructure for large graph-of-convex-sets planning relaxations.
tags:
  - Optimization Software
  - Graph of Convex Sets
  - Robotics
date: "2026-04-26T00:00:00Z"

external_link: ""

image:
  focal_point: Smart
  caption: Representative GCS benchmark instance families spanning maze, helicopter, shelf, contact-graph, SDP pushing, and bimanual problems.

# links:
#   - type: code
#     url: "https://github.com/AlexandreAmice/gcs_solver"
url_pdf: ""
url_slides: ""
url_video: ""
---

# Motivation

Graph of Convex Sets (GCS) is a powerful modeling framework for planning problems that combine discrete choices with continuous decisions.
A path through the graph selects a sequence of convex regions or modes, while the optimization variables choose continuous states inside those regions.

This makes GCS a natural fit for robotics problems such as motion planning through convex regions, manipulation with contact modes, and mixed discrete-continuous task planning. The challenge is scale. A centralized relaxation can become very large, and the graph structure that made the model natural is no longer fully exploited by a generic conic solve.

# Contribution

VEGA is a decomposition solver for GCS programs written in C++. Instead of solving the full conic relaxation as one monolithic program, the method splits the problem into the pieces already present in the model: a local program at each vertex, a local program at each edge, and a global graph optimization update.

At each iteration, these subproblems can be solved in parallel and then driven toward consensus. This creates a solver architecture that matches the original modeling structure and can scale to very large problems.

In addition to VEGA, we provide a benchmark of GCS instances from the literature and distribute these instances as `GcsBench`. We provide new C++ and Python based infrastructure in `GcsCpp` for modelling, serializing, and deserializing instances so that other researchers can contribute their own instances to the benchmark. We also provide bridges to transform `Drake's` GraphOfConvexSets objects and `gcsopt` models to the standardized `GcsCpp` instances.

The benchmark set includes maze navigation, helicopter flight, shelf planning, bimanual manipulation, semidefinite pushing, and contact-graph instances. These programs take anywhere from less than a second to tens of minutes to solve with general-purpose convex solvers. The contact-graph instances are too large to be solved in a reasonable time by general-purpose methods.

# Results

VEGA is designed to solve GCS instances where the convex relaxation is too large to solve using a general-purpose, centralized solver.

It is the only solver in the benchmark capable of solving any of the contact-graph instances.
On problems where centralized solvers do succeed, VEGA is typically slower as the additional overhead of coordinating the local solvers outweighs any benefits from using the decomposition-based method.
