---
title: Radio Amateurs
layout: default
parent: History
has_toc: true
description: A list of radio amateurs that have been an EARS member or been trained by us.
---

{% include math.html %}

<h1><b><span style="color:Gold">Radio Amateur Wall of Fame</span></b></h1>

A list of the Radio Amateurs that have been a member of **EARS** or have been trained by us:

<ul>
{% for member in site.data.members %}
  <li>
    <b><a href="https://www.qrz.com/db/{{ member.callsign }}">{{ member.callsign }}</a></b> - {% if member.name %} {{ member.name }} {% endif %} {% if member.role %} ({{ member.role }}) {% endif %}
  </li>
{% endfor %}
</ul>