---
title: Kapitel
icon: fas fa-book
order: 3
---

## 📘 Unterrichtskapitel & Skripten

Hier findest du alle Kapitel aus meiner Sammlung  
(`_docs/`-Ordner im Repository).

---

{% assign items = site.docs | sort: "title" %}
<ul>
{% for d in items %}
  <li>
    <a href="{{ d.url | relative_url }}">{{ d.title }}</a>
    {% if d.categories and d.categories.size > 0 %}
      <em> – {{ d.categories | join: " / " }}</em>
    {% endif %}
  </li>
{% endfor %}
</ul>

---

> 💡 **Tipp:**  
> Neue Kapitel einfach als `.md`-Datei in `_docs/` anlegen – sie erscheinen hier automatisch nach dem nächsten Build.
