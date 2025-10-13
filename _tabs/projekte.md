---
title: Projekte
icon: fas fa-project-diagram
order: 5
---

{% assign all = site.docs | where:"section","projekte" %}
{% assign roots = all | where_exp:"d","d.path contains '/projekte/' and d.path contains '/index.md'" %}
{% for p in roots %}
- [{{ p.title }}]({{ p.url | relative_url }}) — {{ p.summary }}
{% endfor %}
