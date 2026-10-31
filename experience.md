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

## Volunteering

{% for v in site.data.volunteering %}
<div class="entry">
<h3>{{ v.title }}, {{ v.org }}</h3>
<p class="meta">{{ v.dates }}</p>
<ul>{% for p in v.points %}<li>{{ p }}</li>{% endfor %}</ul>
</div>
{% endfor %}
