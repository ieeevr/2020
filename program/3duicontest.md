---
layout: default
title: Contest Entries
menu:
    name: 3DUI Contest Entries
    parent: Program
    position: 8
permalink: /program/3dui-contest.html
---

# 3DUI Contest Entries

{% for paper in site.data.threeduicontest %}
### {{ paper.Title }}

{% include join-authors.html paper=paper %}

{% if paper.Abstract != Nil %}
Abstract: &ldquo;{{ paper.Abstract }}&rdquo;
{% endif %}

{% unless forloop.last %}
---
{% endunless %}

{% endfor %}