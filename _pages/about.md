---
permalink: /
title: "About Me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am an undergraduate student at the [University of Notre Dame](https://www.nd.edu), majoring in **Computer Science** and **Mathematics**.

I am passionate about artificial intelligence, machine learning, web development, database systems, data science, and statistics. You can view my resume [here]().

Work Experience
-----
I previously interned at [Ford Motor Company](https://www.ford.com) as a **Full Stack Software Engineer**, where I contributed to the development of the Dealer Information System (DIS) online application.

This coming Summer 2024, I am excited to be an incoming software engineer intern for [Garmin](https://www.garmin.com), looking forward to gaining more hands-on experience in the field.

Research
-----
Currently, I work with [Prof. Meng Jiang](http://www.meng-jiang.com/) and PhD student [Noah Ziems](https://noahziems.com/), focusing on various **Large Language Model (LLM)** applications. I helped to introduce a framework that leverages LLMs to enhance the effectiveness of decision tree explanations.

Here are my current **publications**:

{% for pub in site.publications reversed %}
  <div>
    <a style="font-size: medium; display: block;" href="{{ pub.arxivurl }}"><strong>{{ pub.title }}</strong></a>
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

Contact Info
------
You can email me at jflanag5 [AT] nd [DOT] edu, or connect with me on [LinkedIn](https://www.linkedin.com/in/johnflanag/).
