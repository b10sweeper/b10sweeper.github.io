---
layout: default
body_class: home
---
<section class="hero">
<h1 class="hero-name">{{ site.title }}</h1>
<p class="hero-tag">{{ site.description }}</p>
</section>

<section class="wrap selected">
<h2 class="section-title">Selected writing</h2>
<ul class="pieces">
{% for p in site.data.work limit: 3 %}
<li><a href="{{ p.url }}"><span class="piece-title">{{ p.title }}</span><span class="piece-meta">{{ p.outlet }}, {{ p.year }}</span></a></li>
{% endfor %}
</ul>
<p class="more"><a href="{{ '/work/' | relative_url }}">See all work</a></p>
</section>
