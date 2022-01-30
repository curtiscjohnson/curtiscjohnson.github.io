---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
header:
  og_image: ""
---


This is conglomeration of various personal and class projects. 

<nbsp>

{% include base_path %}

{% assign ordered_pages = site.projects | sort:"display_order" %}

{% for post in ordered_pages %}
  {% include archive-single.html %}
{% endfor %}
