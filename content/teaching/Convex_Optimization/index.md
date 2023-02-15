---
title: "6.S098, IAP 2022 -- Applied Convex Optimization"
collection: teaching
type: "Graduate Course"
venue: "MIT"
permalink: /courses/6.S098/
date: 2021-01-22
---
<!-- ---
layout: archive
title: "6.S098, IAP 2022 -- Applied Convex Optimization"
permalink: /courses/6.S098/
author_profile: true
--- -->

**Instructors:** [Alexandre Amice](mailto:amice@mit.edu), [Benoit Legat](mailto:blegat@mit.edu)

**Lectures:** Tuesday/Thursday 1:00-2:30pm January 4th - January 27th

**Syllabus**: [Syllabus](6.S098_Syllabus.pdf)

**Piazza**: [Piazza](http://piazza.com/mit/other/6s098)

**Lecture Recordings**: [Lecture Recordings](https://www.youtube.com/playlist?list=PL5SG6ajT9NZKxdvM1jQOLXmeKO7MfyLxR)



## Course description
Optimization is a cornerstone of many disciplines in engineering. Surprisingly, many problems such
as balancing bipedal robots, designing your own index fund, and allocating power in the energy
grid can be formulated as convex optimization problems. Convex optimization is a mature technology which can be used to solve a huge number of applied problems and can be scaled to problems
with millions of variables. However, recognizing what can be transformed into a convex optimization problem can be challenging. This course will teach you how to recognize, formulate, and solve
these problems.

Lectures will be motivated by realistic case studies from areas where convex optimization is used in
practice. We will briefly survey theoretical results in convex analysis, but the majority of the course
will focus on formulating and solving problems that come up in practice. Applications will include
robotics, signal processing, statistics and machine learning, finance, control, power systems, and
other areas based on student interest. This course is designed for advanced undergraduates and
beginning graduate students.

## Course objectives
- learn to recognize and formulate convex optimization problems that appear in various fields.
- become comfortable using open source software to solve these optimization problems.
- develop insight to decide which solver is best for your problem.
- give students the background needed to feel comfortable in applying these methods in their own research work and/or applications


## About the Course
### Prerequisites
Comfort with multivariable calculus (18.02) and linear algebra (18.06) as well as basic programming in Python or Julia. Familiarity with basic probability and/or controls will aid in understanding many of the case studies.

### Intended audience
Anyone who expects to use optimization as a tool for scientific computing. Beginning graduate and advanced undergraduate students are the particular target audience.


### Schedule
The following schedule is tentative and subject to change.  See Syllabus for in depth topic list. Homework problems will be drawn primarily from [Boyd's Extra Exercises](6.S098_homeworks/boyd_extra_exercises.pdf).

| Date          | Topic          | Homework |
Week 1 01/04, 01/06 | Linear Programming, Fundamentals of Convex Programming   | [Homework 1](6.S098_homeworks/hwmk1.pdf) |
Week 2 01/11, 01/13 | Quadratic and Second Order Cone Programming, Duality |  [Homework 2](6.S098_homeworks/hwmk2.pdf) |
Week 3 01/18, 01/20 | Case Study: Machine Learning and Statistics<br /> Case Study: Power Systems and Bender's Decomposition|  [Homework 3](6.S098_homeworks/hwmk3.pdf) |
Week 4 01/25, 01/27| Hard Optimization Problems: TBD | [Project](6.S098_homeworks/final_project_description.pdf)  |

### Problem Sets
There will be three problem sets, assigned on Wednesday and due the subsequent Wednesday. Grading will be very coarse--emphasis is put on understanding the concepts over correct answers. Problem sets will focus on giving students practice formulating convex optimization problems and obtaining familiarity with solving those programs using open source software.

Each problem set will ask you to model and solve convex optimization problems that come from various application areas, which will be chosen based on interests of the class. Problem sets will require use of the Julia or Python programming languages, but no prior experience in either is required. Problem sets are expected to take around 4 hours each.

### Project
There will be a course project during the last week of IAP that will allow you to apply convex optimization to a problem of interest. The final product will be a short mathematical description of this problem (akin to the descriptions you see on the problem sets) and a solution. Course grading is designed such that this project can take the place of the final problem set. Presentation of the results to the class are a possibility.

### Textbook
The textbook is Convex Optimization by Boyd and Vandenberghe, available [online](https://web.stanford.edu/~boyd/cvxbook/).


### Software
You will use CVX in one of [Python](https://www.cvxpy.org/CVXPY) or [Julia](http://convexjl.readthedocs.org/Convex.jl)

### Grading
- This course is offered for 6 units of credit, and the grading is P/D/F. To receive credit, you must get 16 or more points. A minimum of 4 points of attendance and 2 points on the final project are
required to pass. The main goal of this course is to learn about optimization and solve some fun problems.

Problem Sets | 12 | 4 points per problem set |
Attendance | 6 | 1 point per lecture in person, 0.75 for remote attendance |
Project | 4 |
Total | 22
