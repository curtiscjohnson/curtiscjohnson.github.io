---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
header:
  og_image: ""
---


This is conglomeration of various personal, class, or reaseach projects. Research projects often turn into papers so check out my [publications page](https://curtiscjohnson.github.io/publications/) as well.

More project pages are to come:

  * Apollo CSM Simulation
  * MRAC Notebook
  * RRT obstacle avoidance with Baxter
  * MuJoCo modeling
  * Mars Rover Arm Design
  * Fixed Wing UAV Simulator
  * DH Parameter Optimization

<nbsp>

{% include base_path %}

{% assign ordered_pages = site.projects | sort:"display_order" %}

{% for post in ordered_pages %}
  {% include archive-single.html %}
{% endfor %}
