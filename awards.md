---
layout: default
title: Awards
permalink: /awards/
---

# Awards and recognition

{% for a in site.data.awards %}
<div class="entry">
<h3>{{ a.title }}</h3>
<p class="meta">{{ a.issuer }} · {{ a.date }}</p>
{% if a.note %}<p>{{ a.note }}</p>{% endif %}
</div>
{% endfor %}
