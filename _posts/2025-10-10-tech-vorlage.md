---
title: TECH-Vorlage
date: 2025-10-10 10:00:00 +0200
categories: [Tech, How-To]
tags: [chirpy, jekyll, tutorial, code]
description: Vorlage für technische Blogposts mit Code, Formeln, Diagrammen.
image:
  path: /assets/img/cover-tech.png
  alt: Tech Cover
pin: false
mermaid: true
---

## Zusammenfassung
Kurzer Überblick in 2–3 Sätzen: Was lernen Leser:innen? Welche Voraussetzungen?

---

## Voraussetzungen
- Grundkenntnisse in …
- Installiertes: `python >= 3.11`, `git`, `make`

---

## TL;DR (Schnellstart)
```bash
# 1) Projekt klonen
git clone https://example.com/repo.git
cd repo

# 2) Setup
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

# 3) Start
make run

Hintergrund
Warum ist das relevant? Welche typischen Probleme löst der Beitrag?
Schritt-für-Schritt Anleitung
Schritt 1 – Setup prüfen
python --version
Erwarte 3.11.x. Falls nicht, verweise auf Installation.
Schritt 2 – Minimalbeispiel
# hello.py
def hello(name: str) -> str:
    return f"Hello, {name}!"

if __name__ == "__main__":
    print(hello("World"))
Ausführen:
python hello.py
Schritt 3 – Test hinzufügen
# test_hello.py
from hello import hello

def test_hello():
    assert hello("World") == "Hello, World!"
Formeln
Inline $E = mc^2$ oder als Block:
$ ∇⋅F⃗=ρ∇⋅F =ρ $

Diagramm (Mermaid)
flowchart LR
  A[Input] --> B[Verarbeitung]
  B --> C{Ergebnis ok?}
  C -- Ja --> D[Deploy]
  C -- Nein --> E[Fehler beheben]
Benchmarks / Tabelle
Fall	Dauer [ms]	Kommentar
A	12	Warm Cache
B	37	Kaltstart
C	22	Optimiert
Häufige Fehler (FAQ)
Build bricht ab? Prüfe Gemfile.lock/Ruby-Version.
Mermaid rendert nicht? mermaid: true im Frontmatter setzen.
Fazit
Kurzresümee + ggf. Ausblick auf weiterführende Themen/Links.

