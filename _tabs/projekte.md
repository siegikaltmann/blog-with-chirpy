---
title: Projekte
icon: fas fa-project-diagram
order: 5
permalink: /projekte/
---

{% for p in site.projects %}
  {% assign parts = p.path | split:'/' %}
  {%- comment -%}
    _projects/<slug>/index.md  => parts.size == 3
    _projects/<slug>/<sub>/index.md => parts.size >= 4  (ausblenden)
  {%- endcomment -%}
  {% if parts.size == 3 and parts[0] == '_projects' and parts[2] == 'index.md' %}
- [{{ p.title }}]({{ p.url | relative_url }}) — {{ p.summary }}
  {% endif %}
{% endfor %}
