---
layout: page
title: Docs
icon: fas fa-book
order: 2
---

Hier findest du alle Dokumentationsseiten.

<ul>
{% for p in site.docs %}
  <li><a href="{{ p.url | relative_url }}">{{ p.title | default:p.path }}</a></li>
{% endfor %}
</ul>
