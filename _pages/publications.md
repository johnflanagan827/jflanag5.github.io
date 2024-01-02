---
layout: archive
title: ""
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

# Publications

{% for pub in site.publications reversed %}
  <div>
    <a style="font-size: large; display: block;" href="{{ pub.arxivurl }}"><strong>{{ pub.title }}</strong></a>
    <p style="font-size: medium; margin-top: 6px; margin-bottom: 1px;">
      {% assign authors = pub.authors | split: "," %}
      {% assign authors_list = '' %}

      {% for author in authors %}
      {% assign trimmed_author = author | strip %}
      {% if trimmed_author == site.author.name %}
      {% assign formatted_author = '<strong>' | append: trimmed_author | append: '</strong>' %}
      {% else %}
      {% assign formatted_author = trimmed_author %}
      {% endif %}
      
      {% if forloop.last == false %}
      {% assign authors_list = authors_list | append: formatted_author | append: ', ' %}
      {% else %}
      {% assign authors_list = authors_list | append: formatted_author %}
      {% endif %}
      {% endfor %}
      
      {{ authors_list }}

    </p>

    <p style="font-size: medium; margin-top: 0;">
      <i>{{ pub.venue }}</i> 
      {% if pub.link %}
        <a href="{{ pub.link }}" title="Publication Link"><i class="fas fa-fw fa-link zoom" aria-hidden="true"></i></a>
      {% endif %}
      {% if pub.paperurl %}
        <a href="{{ pub.paperurl }}" title="Download PDF"><i class="fas fa-fw fa-file-pdf zoom" aria-hidden="true"></i></a>
      {% endif %}
      {% if pub.codeurl %}
      <a href="{{ pub.codeurl }}" title="GitHub Code"><i class="fab fa-fw fa-github zoom" aria-hidden="true"></i></a>
      {% endif %}
    </p>
  </div>
{% endfor %}

