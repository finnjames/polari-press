---
layout: default
title: Polari Press Catalogue
permalink: /catalogue
---

### Catalogue

<div id="catalogue">
  {% for item in site.data.catalogue %}
  <div class="book" style="border-color: {% cycle '#a82e1e', '#ffd149', '#199e0f', '#1a4fcc' %}">
    <div>
      <h1>{{ item.title }}</h1>
      {% if item.subtitle %}
        <h2>{{ item.subtitle }}</h2>
      {% endif %}
    </div>
    <h3>{{ item.author }}</h3>
  </div>
  {% endfor %}
</div>