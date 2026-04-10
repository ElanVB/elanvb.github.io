---
layout: default
title: Home
---

<div class="hero">
  <p class="eyebrow">Hello</p>
  <h1>{{ site.title }}</h1>
  <p class="intro">{{ site.description }}</p>
</div>

<div class="links-grid">
  {% raw %}{% for link in site.data.links %}{% endraw %}
    <a class="link-card" href="{% raw %}{{ link.url }}{% endraw %}">
      <h2>{% raw %}{{ link.title }}{% endraw %}</h2>
      <p>{% raw %}{{ link.description }}{% endraw %}</p>
      <span class="link-arrow">Open →</span>
    </a>
  {% raw %}{% endfor %}{% endraw %}
</div>