---
title: Diplomarbeit – <Titel>
section: projekte
project: diplomarbeit
summary: Kurzbeschreibung in 1–2 Sätzen.
start: 2025-09-01
due: 2026-02-28
status: active
---

## Schnellzugriff
- [Gantt & Fortschritt](./gantt/)
- [Alle Meetings](./meetings/)
- [Zwischenberichte](./berichte/)

## Nächste Meetings
{% assign pdocs = site.docs | where:"section","projekte" | where:"project","diplomarbeit" %}
{% assign meetings = pdocs | where:"type","meeting" | sort:"date" %}
{% for m in meetings limit:3 %}
- {{ m.date | date: "%d.%m.%Y %H:%M" }} — [{{ m.title }}]({{ m.url | relative_url }})
{% endfor %}

## Letzte Berichte
{% assign reports = pdocs | where:"type","report" | sort:"date" | reverse %}
{% for r in reports limit:2 %}
- {{ r.date | date: "%d.%m.%Y" }} — [{{ r.title }}]({{ r.url | relative_url }})
{% endfor %}

