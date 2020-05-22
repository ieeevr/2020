---
layout: default
title: Papers
menu:
    name: Papers
    parent: Program
    position: 4
permalink: /program/papers.html
---

# TVCG Papers

{% for paper in site.data.papers %}
- [{{ paper.Title }}](#tvcg-{{ forloop.index }})
{% endfor %}

# TVCG Invited Papers

{% for paper in site.data.invited-papers %}
- [{{ paper.Title }}](#tvcg-invited-{{ forloop.index }})
{% endfor %}

# Conference Papers

{% for paper in site.data.conference-papers %}
- [{{ paper.Title }}](#conference-{{ forloop.index }})
{% endfor %}

---

{% for paper in site.data.papers %}
<a id="tvcg-{{ forloop.index }}" class="anchor"></a>
### {{ paper.Title }}

{% include join-authors.html paper=paper %}

{: .text-muted .small}
TVCG

{% if paper.Abstract != Nil %}
Abstract: &ldquo;{{ paper.Abstract }}&rdquo;
{% endif %}

{% endfor %}

{% for paper in site.data.invited-papers %}
<a id="tvcg-invited-{{ forloop.index }}" class="anchor"></a>
### {{ paper.Title }}

{% include join-authors.html paper=paper %}

{: .text-muted .small}
TVCG Invited

{% if paper.Abstract != Nil %}
Abstract: &ldquo;{{ paper.Abstract }}&rdquo;
{% endif %}

{% endfor %}

{% for paper in site.data.conference-papers %}
<a id="conference-{{ forloop.index }}" class="anchor"></a>
### {{ paper.Title }}

{% include join-authors.html paper=paper %}

{: .text-muted .small}
Conference

{% if paper.Abstract != Nil %}
Abstract: &ldquo;{{ paper.Abstract }}&rdquo;
{% endif %}

{% endfor %}