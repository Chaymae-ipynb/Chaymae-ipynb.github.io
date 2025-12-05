---
layout: default
title: Research
permalink: /research/
---

# Research Projects

<div class="research-list">

{% for page in site.pages %}
  {% if page.path contains 'research/' and page.path != 'research.md' and page.title %}
  
  <a href="{{ page.url }}" class="research-card">
    <div class="card-content">
      <h2 class="card-title">{{ page.title }}</h2>
      <p class="card-summary">{{ page.summary }}</p>
      <p class="card-date">{{ page.date | date: "%B %d, %Y" }}</p>
    </div>
  </a>

  {% endif %}
{% endfor %}

</div>
