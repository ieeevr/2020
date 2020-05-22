---
layout: default
title: Research Demonstrations
menu:
    name: Research Demos
    parent: Program
    position: 10
permalink: /program/demos.html
---

# Research Demos

{% assign accepted-papers = site.data.research-demos | where:"Submission Complete","Yes" %}

{% assign session1-papers = accepted-papers | where:"Days","1 & 2" %}
{% assign session2-papers = accepted-papers | where:"Days","3 & 4" %}

## Days 1 and 2

{% for paper in session1-papers %}
Demo ID: {{ paper.ID }}
### {{ paper.Title }}

{{ paper.Authors }}

{{ paper.Affiliation }}

{% if paper.Abstract != Nil %}
Abstract: &ldquo;{{ paper.Abstract }}&rdquo;
{% endif %}

{% unless forloop.last %}
---
{% endunless %}

{% endfor %}

## Days 3 and 4

{% for paper in session2-papers %}
Demo ID: {{ paper.ID }}
### {{ paper.Title }}

{{ paper.Authors }}

{{ paper.Affiliation }}

{% if paper.Abstract != Nil %}
Abstract: &ldquo;{{ paper.Abstract }}&rdquo;
{% endif %}

{% unless forloop.last %}
---
{% endunless %}

{% endfor %}