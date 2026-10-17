---
layout: default
title: Work
permalink: /work/
---
<div class="wrap">
<ul class="pieces">
{% for p in site.data.work %}
<li><a href="{{ p.url }}"><span class="piece-title">{{ p.title }}</span><span class="piece-meta">{{ p.outlet }}, {{ p.year }}</span></a></li>
{% endfor %}
</ul>
</div>
