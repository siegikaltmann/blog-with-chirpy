---
title: Hinweisboxen (RealPython-Stil)
date: 2025-10-12 20:00:00 +0200
categories: ui
tags: [admonition, notes]
toc: true
---

## Info

{% capture body %}
So setzt du **Info-Kästchen** im RealPython-Look.
Du kannst hier ganz normal **Markdown** verwenden.
{% endcapture %}
{% include admonition.html type="info" title="Hinweis" content=body %}

---

## Success

{% capture body %}
Alles hat **geklappt**! 🎉  
Auch Listen gehen:
- Punkt A
- Punkt B
{% endcapture %}
{% include admonition.html type="success" title="Erfolgreich" content=body %}

---

## Warning

{% capture body %}
**Achtung:** Bitte vorher sichern.
{% endcapture %}
{% include admonition.html type="warning" title="Achtung" content=body %}

---

## Danger

{% capture body %}
**Fehler:** Etwas ist schiefgelaufen. Bitte Eingaben prüfen.
{% endcapture %}
{% include admonition.html type="danger" title="Fehler" content=body %}

---

## Note (neutral)

{% capture body %}
Kleine **Notiz** am Rand – neutraler Hinweis ohne besondere Semantik.
{% endcapture %}
{% include admonition.html type="note" title="Notiz" content=body %}
