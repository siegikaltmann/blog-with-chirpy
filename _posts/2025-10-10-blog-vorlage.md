---
title: BLOG-Vorlage
date: 2025-10-10 10:00:00 +0200
categories: [Blog, Vorlage]
tags: [template, chirpy, markdown]
description: Eine Vorlage für zukünftige Blogbeiträge im Chirpy-Theme.
image:
  path: /assets/img/winter_wonder_land_bw.heic
  alt: Beispiel-Coverbild
---

## Einleitung

<style>
.note{padding:1rem 1.25rem;margin:1.2rem 0;border-left:6px solid transparent;border-radius:.75rem;box-shadow:0 4px 12px rgba(0,0,0,.05)}
.note-danger{background:#fee2e2;border-color:#dc2626;color:#7f1d1d}
</style>
<div class="note note-alert">Test-Box</div>


Hier beginnt dein Text. Beschreibe kurz, worum es in diesem Beitrag geht.  
Du kannst **Markdown**, $\LaTeX$, Codeblöcke und Bilder verwenden.

---
<div class="note note-danger">
🚨 <strong>Danger:</strong> Jetzt sollte die Box sichtbar sein.
</div>


---

## Abschnitt 1 – Beispielüberschrift

Hier steht ein Absatz mit etwas Fließtext.  
Markdown unterstützt *kursiv*, **fett** und `Code`.

```python
# Beispiel-Codeblock
def hallo():
    print("Hallo, Welt!")
```
<div class="note note-danger">
🚨 <strong>Danger:</strong> Box sollte jetzt gestylt sein.
</div>

<div class="note-test">
🧪 Testbox: Gelb mit schwarzem Streifen.
</div>


## Abschnitt 2 – Formeln
Du kannst auch mathematische Ausdrücke einfügen:
$\sum{}F=0, \sum{}M=0$


## Abschnitt 3 – Bilder
Ein Bild aus deinem Ordner /assets/img/ einfügen:

![Vorarlberger Alpen](/assets/img/winter_wonder_land_bw.heic){: style="float: left; margin: 0 1rem 1rem 0;" width="300" .shadow .rounded }


## Abschnitt 4 – Fazit
Kurzes Fazit oder Ausblick.
„Ein guter Post endet mit einem Gedanken, der hängen bleibt.“


## Frontmatter-Erklärung
Schlüssel	Bedeutung
title	Titel des Blogposts
date	Veröffentlichungsdatum
categories	Hierarchische Einordnung (z. B. [Blog, Technik])
tags	Stichworte
description	Kurzbeschreibung für Suchmaschinen
image.path	Pfad zum Titelbild
image.alt	Alternativtext für das Bild

💡 Tipp:
Wenn du einen neuen Beitrag erstellen willst, kopiere einfach diese Datei und ändere:
title, date, categories, tags, description
Textinhalte darunter

## Callouts mittels html

<div style="background:#e6ffed; border-left:6px solid #22c55e; padding:1em; border-radius:0.5em;">
  ✅ <strong>Success:</strong> Alles hat funktioniert!
</div>

<div style="background:#fff2f2; border-left:6px solid #ef4444; padding:1em; border-radius:0.5em;">
  ⚠️ <strong>Danger:</strong> Etwas ist schiefgelaufen.
</div>

## Callouts mittels selbstdefinierten Boxen in assets/css/custom.scss
/* Allgemeiner Stil */
.alert {
  padding: 1em 1.2em;
  border-radius: 0.5em;
  margin: 1em 0;
  color: #0b1020;
  font-weight: 500;
}

/* Varianten */
.alert-info {
  background: #e0f2fe;
  border-left: 6px solid #0ea5e9;
}
.alert-success {
  background: #dcfce7;
  border-left: 6px solid #22c55e;
}
.alert-warning {
  background: #fef9c3;
  border-left: 6px solid #eab308;
}
.alert-danger {
  background: #fee2e2;
  border-left: 6px solid #ef4444;
}

<div class="alert alert-info">
💡 **Info:** Du kannst Markdown *innerhalb* der Box verwenden!
</div>

<div class="alert alert-danger">
⚠️ **Fehler:** Überprüfe deine Frontmatter-Daten.
</div>

## Callout mit Admonition im custom.scss

.admonition {
  padding: 1em;
  margin: 1em 0;
  border-radius: 0.5em;
  border-left: 5px solid;
}

.admonition.info    { background: #e0f2fe; border-color: #0ea5e9; }
.admonition.warning { background: #fef9c3; border-color: #eab308; }
.admonition.danger  { background: #fee2e2; border-color: #ef4444; }
.admonition.success { background: #dcfce7; border-color: #22c55e; }

<div class="admonition info">
💡 <strong>Info:</strong> Das ist eine Info-Box im Dokumentationsstil.
</div>

<div class="admonition danger">
🚨 <strong>Danger:</strong> Diesen Befehl nur mit Vorsicht ausführen!
</div>


<div class="note note-info">
💡 <strong>Info:</strong> Du kannst Markdown innerhalb dieser Box nutzen.
</div>

<div class="note note-success">
✅ <strong>Success:</strong> Alles hat funktioniert wie geplant.
</div>

<div class="note note-warning">
⚠️ <strong>Warnung:</strong> Überprüfe die Eingabedaten sorgfältig.
</div>

<div class="note note-danger">
🚨 <strong>Fehler:</strong> Die Datei wurde nicht gefunden.
</div>

---
### Einbinden in _sass/custom/styles.scss

<div class="note note-danger">
🚨 <strong>Danger:</strong> Vorsicht mit diesem Befehl!
</div>

<div class="admonition info">
💡 <strong>Info:</strong> So klappt’s zuverlässiger.
</div>

