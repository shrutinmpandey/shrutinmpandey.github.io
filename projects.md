---
layout: default
title: Projects
permalink: /projects/
---

# Projects

Academic projects completed during my B.Tech at VIT Vellore.

{% for p in site.data.projects %}
<div class="entry">
<h3>{{ p.title }}</h3>
<p class="meta">{{ p.dates }}{% if p.course %} · {{ p.course }}{% endif %} · Guide: {{ p.guide }}</p>
</div>
{% endfor %}
