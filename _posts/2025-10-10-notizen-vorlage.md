---
title: NOTIZEN-Vorlage
date: 2025-10-10 10:05:00 +0200
categories: [Notes]
tags: [snippet, memo, tldr]
description: Schlanke Vorlage für schnelle Notizen, Changelogs und Checklisten.
pin: false
mermaid: false
---

## TL;DR
Ein Satz, der die Notiz auf den Punkt bringt.

---

## Kontext
Warum schreibe ich diese Notiz? (max. 2–3 Sätze)

---

## To-do / Checkliste
- [ ] Aufgabe 1
- [ ] Aufgabe 2
- [ ] Aufgabe 3

---

Perfekte Beobachtung 👀 — ja, Chirpy zentriert standardmäßig alle Bilder in Beiträgen.
Das passiert über die CSS-Regel
.post-content img {
  display: block;
  margin: auto;
}
Aber: du kannst das Verhalten ganz leicht überschreiben oder gezielt steuern.
Hier sind alle gängigen Varianten 👇
🖼️ 1. Standard (zentriert)
![Beispiel](/assets/img/winter_wonder_land_bw.heic){: .rounded. .shadow width="300"}
→ Bild wird zentriert dargestellt.
🔹 2. Linksbündig
![Beispiel links](/assets/img/test.png){: .normal .float-left width="300"}
oder (wenn .float-left nicht greift):
![Beispiel links](/assets/img/test.png){: style="float: left; margin: 0 1rem 1rem 0;" }
Damit bleibt Text rechts daneben fließend.
🔹 3. Rechtsbündig
![Beispiel rechts](/assets/img/test.png){: style="float: right; margin: 0 0 1rem 1rem;" }
→ Text läuft links am Bild entlang.
🔹 4. Vollbreit (maximale Seitenbreite)
![Vollbreit](/assets/img/test.png){: .w-100 }
oder falls .w-100 fehlt:
![Vollbreit](/assets/img/test.png){: style="width:100%; height:auto;" }
🔹 5. Zentriert, aber mit Schatten / Rahmen
![Schöner Stil](/assets/img/test.png){: .shadow .rounded .w-75 }
→ bleibt zentriert, aber 75 % Breite, runde Ecken und Schatten (Chirpy-Builtins).
🔹 6. Bild mit Beschriftung (Figure)
<figure>
  <img src="/assets/img/test.png" alt="Beschreibung" width="400">
  <figcaption>Abbildung 1: Beispielhafte Darstellung</figcaption>
</figure>
→ Damit kannst du mit HTML exakter steuern (z. B. Schriftgröße, Ausrichtung).
🔹 7. Eigenes Styling in CSS (optional)
Wenn du es dauerhaft ändern willst, füge z. B. in deine Datei
assets/css/custom.scss (falls noch nicht vorhanden):
/* Beispiel: Bilder standardmäßig linksbündig */
.post-content img {
  display: inline-block;
  margin: 0 1rem 1rem 0;
}

/* oder: zentriert, aber 80 % Breite */
.post-content img {
  display: block;
  margin: 0 auto;
  width: 80%;
}

---

## Snippets
```bash
# Häufig genutzter Befehl
rsync -av --progress src/ user@host:/path/
# Mini-Snippet
from datetime import datetime
print(datetime.now().isoformat())
Quick-Links
Dokumentation
Ticket/Issue
Quelle/Artikel
Changelog
2025-10-10: Notiz erstellt
2025-10-11: Abschnitt Snippets ergänzt
