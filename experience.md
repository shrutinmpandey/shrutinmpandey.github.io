---
layout: default
title: Experience
permalink: /experience/
---

# Experience

{% for job in site.data.experience %}
<div class="entry">
<h3>{{ job.title }}, {{ job.company }}</h3>
<p class="meta">{{ job.dates }}{% if job.location %} · {{ job.location }}{% endif %}</p>
{% if job.points %}<ul>{% for p in job.points %}<li>{{ p }}</li>{% endfor %}</ul>{% endif %}
</div>
{% endfor %}
