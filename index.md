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
  {% for link in site.data.links %}
    <a class="link-card" href="{{ link.url }}">
      <h2>{{ link.title }}</h2>
      <p>{{ link.description }}</p>
      <span class="link-arrow">Open →</span>
    </a>
  {% endfor %}
</div>