---
title: "Diplomarbeit – Paketsortieranlage 25-26"
project: diplomarbeit
summary: "Farbsensor aktive Paketsortieranlage gesteuert von Raspberry Pi Pico 2, programmiert in MicroPython"
start: 2025-09-01
due: 2026-06-28
status: active
permalink: /projekte/diplomarbeit/   # <— wichtig für die Startseite
---

## Schnellzugriff
- [Gantt & Fortschritt](./gantt/)
- [Alle Meetings](./meetings/)
- [Zwischenberichte](./berichte/)


## Nächste Meetings
{% assign pitems = site.projects | where: "project", "diplomarbeit" %}
{% assign meetings = pitems | where: "type", "meeting" | sort: "date" %}
{% for m in meetings limit:3 %}
- {{ m.date | date: "%d.%m.%Y %H:%M" }} — [{{ m.title }}]({{ m.url | relative_url }})
{% else %}
- *(Derzeit keine Meetings erfasst.)*
{% endfor %}

## Letzte Berichte
{% assign reports = pitems | where: "type", "report" | sort: "date" | reverse %}
{% for r in reports limit:2 %}
- {{ r.date | date: "%d.%m.%Y" }} — [{{ r.title }}]({{ r.url | relative_url }})
{% else %}
- *(Noch keine Zwischenberichte.)*
{% endfor %}
