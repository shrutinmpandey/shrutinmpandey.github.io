---
layout: default
title: Education
permalink: /education/
---

# Education

{% for e in site.data.education %}
<div class="entry">
<h3>{{ e.school }}</h3>
<p class="meta">{{ e.degree }} · {{ e.dates }}{% if e.grade %} · {{ e.grade }}{% endif %}</p>
{% if e.points %}<ul>{% for p in e.points %}<li>{{ p }}</li>{% endfor %}</ul>{% endif %}
</div>
{% endfor %}

## Certifications

{% for c in site.data.certifications %}
<div class="entry">
<h3>{{ c.title }}</h3>
<p class="meta">{{ c.issuer }} · {{ c.date }}</p>
</div>
{% endfor %}
