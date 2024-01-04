---
layout: archive
title: ""
permalink: /projects/
author_profile: true
---

# Personal Projects

Here are several personal projects I created independently, which have helped improve my coding practices and learn new technologies.

{% for post in site.personal-projects reversed %}
{% include archive-single.html %}
{% endfor %}

--- 

# Academic Projects

Below are a selection of personal projects I completed during my class. While it's not an exhaustive list, it primarily features open-ended creative assignments.

{% for post in site.academic-projects reversed %}
{% include archive-single.html %}
{% endfor %}
