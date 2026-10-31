---
layout: default
title: Projects
permalink: /projects/
---

# Projects

{% for p in site.data.projects %}
<div class="entry">
<h3>{{ p.title }}</h3>
<p class="meta">{{ p.dates }}{% if p.context %} · {{ p.context }}{% endif %}</p>
{% if p.contributors or p.skills %}<ul>
{% if p.contributors %}<li>Contributors: {{ p.contributors }}</li>{% endif %}
{% if p.skills %}<li>Skills: {{ p.skills }}</li>{% endif %}
</ul>{% endif %}
</div>
{% endfor %}
