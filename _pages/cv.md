---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Ph.D in Electrical Engineering and Computer Science, Massachusetts Institute of Technology, (2020- present)
* M.S.E in Robotics, University of Pennsylvania, (2016-2020)
* B.S.E. in Electrical Engineering and Mathematics, University of Pennsylvania, (2016-2020)

Work experience
======
* <b>Uber Advanced Technology Group:</b> Machine Perception Intern (Summer 2019)
  * Designed and implemented a novel radar tracking algorithm in Python enabling the radar to perform instance segmentation. Decreased the time from first detection to full-state estimation of vehicles by a actor of six
  * Refactored C++ based radar tracking pipeline to allow sensor fusion across radars. Improved performance on proprietary metrics by 20% while reducing computational overhead.

* <b>Alelab:</b> Research Assistant (Winter 2018 - Summer 2020)
  * Studied the application of tools in combinatorial and convex optimization to problems in control theory.
  * Published two conference papers and one journal paper
  * Advisor: Alejandro Ribeiro

* <b>Daugherty Business Solutions:</b> Software Engineering Intern (Summer 2017)
  * Created a rapid prototyping platform to enable the creation of custom apps on top of Amazon Alexa to demonstrate the company's capabilities to develop custom solutions.
  * Created a virtual office receptionist capable of informing guests of the location of employees throughout the office by using Bluetooth sensors located in the office by using this platform.
  
Programming Languages
======
* Python (expert)
  * PyTorch
  * OpenCV
  * CVX
* C++ (proficient)

Languages
=====
* English (native speaker)
* French (native speaker)
* Spanish (proficient)

Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
<!-- Talks
======
  <ul>{% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>
   -->
   
Teaching
======
  <ul>{% for post in site.teaching %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
* Hack MIT Beginner Mentor
* MIT Graduate Application Assistance Program
* University of Pennsylvania ESE Graduate Application Assistance Program
