---
title: "Meetings"
project: diplomarbeit
layout: page
permalink: /projekte/diplomarbeit/meetings/
toc: false
---

{% assign pitems = site.projects | where: "project", "diplomarbeit" %}
{% assign meetings = pitems | where: "type", "meeting" | sort: "date" %}

## Nächste Meetings
{% assign upcoming = meetings | where_exp:"m","m.date >= site.time" %}
{% if upcoming.size > 0 %}
{% for m in upcoming %}
- {{ m.date | date: "%d.%m.%Y %H:%M" }} — [{{ m.title }}]({{ m.url | relative_url }}){% if m.location %} ({{ m.location }}){% endif %}
{% endfor %}
{% else %}
- *(keine kommenden Meetings erfasst)*
{% endif %}

## Vergangene Meetings
{% assign past = meetings | where_exp:"m","m.date < site.time" | reverse %}
{% if past.size > 0 %}
{% for m in past %}
- {{ m.date | date: "%d.%m.%Y %H:%M" }} — [{{ m.title }}]({{ m.url | relative_url }})
{% endfor %}
{% else %}
- *(noch keine vergangenen Meetings)*
{% endif %}
