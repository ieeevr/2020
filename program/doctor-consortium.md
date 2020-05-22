---
layout: default
title: Doctoral Consortium
menu:
    name: Doctoral Consortium
    parent: Program
    position: 11
permalink: /program/doctoral-consortium.html
---

# Doctoral Consortium

The DC is a concentrated full-day event where students present their research interests/plans/results to a panel of senior researchers in the field and receive specific constructive feedback, followed by a reception in the evening and networking opportunities during the following days. Accepted students will give in-depth presentations of their research and will receive constructive comments from mentors. Additionally, accepted students will create a poster about their work to allow IEEE VR attendees to quickly familiarize themselves with each other’s work and to be shown to a broader audience during the conference poster session.

### Accepted Students

<table class="table table-striped">
    <thead>
        <tr>
            <th>Student</th>
            <th>Title</th>
            <th>Affiliation</th>
        </tr>
    </thead>
    <tbody>
{% for paper in site.data.dc %}
<tr>
<td>{{ paper['Contact Name'] }}</td>
<td>{{ paper.Title }}</td>
<td>{{ paper.Affiliation }}</td>
</tr>
{% endfor %}
    </tbody>
</table>