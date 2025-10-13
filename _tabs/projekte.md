---
title: Projekte
icon: fas fa-project-diagram
order: 5
---

{% for p in site.projects %}
  {% if p.path contains '/index.md' %}
- [{{ p.title }}]({{ p.url | relative_url }}) — {{ p.summary }}
  {% endif %}
{% endfor %}
