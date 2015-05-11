---
layout: page
title: "members"
footer: true
sidebar: false
---

{% img right-align /images/concertSpring2015.jpg 400 %}

<table>
{% for member in site.member_current %}
<tr><td>{{ member.name }}</td><td>{{ member.part }}</td></tr>
{% endfor %}
</table>

Novis Alumni
------------
<table>
{% for member in site.member_alumni %}
{% cycle 'alumni_start': '<tr>', '', '' %}
<td>{{ member.name }} | {{ member.year }}</td>
{% cycle 'alumni_end': '', '', '</tr>' %}
{% endfor %}
</table>
