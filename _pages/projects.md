---
layout: archive
title: ""
permalink: /projects/
author_profile: true
---

# Personal Projects

Below are several of my personal projects.

{% for post in site.personal-projects reversed %}
{% include archive-single.html %}
{% endfor %}

--- 

# Academic Projects

Below are some personal projects I completed during class. While not an exhaustive list, it primarily features open-ended creative assignments.

{% for post in site.academic-projects reversed %}
{% include archive-single.html %}
{% endfor %}
