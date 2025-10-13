---
title: "Zwischenberichte"
project: diplomarbeit
layout: page
permalink: /projekte/diplomarbeit/berichte/
toc: false
---

{% assign pitems = site.projects | where: "project", "diplomarbeit" %}
{% assign reports = pitems | where: "type", "report" | sort: "date" | reverse %}

{% if reports.size > 0 %}
## Alle Berichte (neueste zuerst)
{% for r in reports %}
- {{ r.date | date: "%d.%m.%Y" }} — [{{ r.title }}]({{ r.url | relative_url }})
{% endfor %}
{% else %}
- *(Noch keine Berichte vorhanden.)*
{% endif %}

[Zur Projektseite](../)
