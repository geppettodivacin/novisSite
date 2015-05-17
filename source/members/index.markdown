---
layout: page
title: "members"
footer: true
sidebar: false
---

<div class="grid">
<div class="col-1-3"/>
<table>
{% for member in site.member_current %}
<tr><td>{{ member.name }}</td><td>{{ member.part }}</td></tr>
{% endfor %}
</table>
</div>
<div class="left-align"/>

{% img middle-vert /images/womenSpring2015.jpg 300 %}
{% img middle-vert /images/menSpring2015.jpg 300 %}

</div>
</div>

Novis Alumni
------------
<table>
{% for member in site.member_alumni %}
{% cycle 'alumni_start': '<tr>', '', '' %}
<td>{{ member.name }} | {{ member.year }}</td>
{% cycle 'alumni_end': '', '', '</tr>' %}
{% endfor %}
</table>
