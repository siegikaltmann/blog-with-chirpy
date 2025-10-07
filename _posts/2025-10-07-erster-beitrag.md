---
title: "Mein erster Beitrag"
date: 2025-10-07 20:00:00 +0200
categories: [Blog, Start]
tags: [chirpy, jekyll, github-pages]
author: siegik
---

Willkommen zu meinem ersten Beitrag auf meiner neuen **Chirpy-Website** 🎉  

Ich teste hier, wie **Markdown**, **Code**, **Bilder** und **Formeln** aussehen.

---

## 💡 Markdown-Beispiele

**Fett**, *kursiv*, `inline-code` und  
eine Liste:

- Punkt 1
- Punkt 2
- Punkt 3

---

## 🧮 Formeln mit LaTeX

Inline: $E = mc^2$

Block:

$$
\sum F = 0 \\
\sum M = 0
$$

---

## 💻 Code-Beispiel

```python
def hallo():
    print("Hallo Welt!")

hallo()
```

🖼️ Bild
Das ist der Anfang 🚀
Im nächsten Schritt kommen weitere Beiträge, Seiten und Farben.

---

## ⚙️ 3. Optional: Autor hinzufügen

Falls du noch **nicht** in `_data/authors.yml` stehst, lege dort folgendes an:

```yaml
siegik:
  name: "Siegfried Kaltmann"
  avatar: "/assets/img/avatar.png"
  url: "https://siegikaltmann.io/blog-with-chirpy"

Nützliche Tipps fürs Weiterarbeiten
Bei Projekt-Seite weiter mit
url: "https://siegikaltmann.github.io"
baseurl: "/blog-with-chirpy"
Neue Inhalte/Änderungen → Commit → Actions baut → Deployment aktualisiert.
Cache-Bypass bei merkwürdigem Verhalten: ?v=now an die URL anhängen.

.
├── _config.yml
├── _posts/
│   ├── 2025-10-07-erster-beitrag.md
│   └── ...
├── _tabs/
│   ├── about.md
│   ├── tags.md
│   └── categories.md
├── _data/
│   └── authors.yml
├── assets/
│   ├── img/
│   └── css/
└── index.html

📝 2. Blogbeiträge hinzufügen (_posts)
Jeder Blogpost ist eine Markdown-Datei mit folgendem Muster:
Dateiname:
YYYY-MM-DD-titel-des-beitrags.md
Beispielinhalt:
---
title: "Mein erster Beitrag"
date: 2025-10-07 14:00:00 +0200
categories: [Blog, Allgemein]
tags: [jekyll, chirpy, test]
---

Willkommen zu meinem ersten Beitrag auf meiner neuen Chirpy-Website 🎉  
Hier teste ich Markdown, LaTeX, Code und mehr.

```python
print("Hallo Welt!")
Inline-Formel: $E = mc^2$
Und ein Bild:

📂 **Ort:** `_posts/2025-10-07-mein-erster-beitrag.md`

---

## 📘 3. Statische Seiten hinzufügen (`_tabs` oder `/`)

### Beispiel: Neue Seite „Projekte“

Lege eine Datei `_tabs/projekte.md` an:

```markdown
---
title: Projekte
icon: fas fa-project-diagram
order: 4
---

Hier sammle ich meine aktuellen Projekte 🚀

- 📘 **Website** mit Jekyll & Chirpy
- 🧠 **Skriptum** in Markdown
- 💻 **Python-Tools**
➡️ Sie erscheint automatisch als neuer Tab in der Navigationsleiste.

👥 4. Autoreninfos (_data/authors.yml)
Beispiel:
siegik:
  name: "Siegfried Kaltmann"
  avatar: "/assets/img/avatar.png"
  url: "https://siegikaltmann.io"
Dann kannst du im Post-Frontmatter z. B. schreiben:
author: siegik
🖼️ 5. Bilder & Medien
Lege deine Bilder hier ab:
assets/img/
Beispiel:
/assets/img/avatar.png
Einbinden in Markdown:
![Beschreibung](/assets/img/avatar.png)
⚙️ 6. Navigation, Titel, Farben usw. (_config.yml)
Dort findest du:
title: Siegikaltmann.io
tagline: "HTL | TGM | Engineering | Python"
lang: de
timezone: Europe/Vienna
Und Tabs aktivieren/deaktivieren:
tabs:
  - about
  - categories
  - tags
  - projekte
🔄 7. Lokales Testen
Falls du lokal testen willst:
bundle exec jekyll serve
Dann im Browser:
👉 http://localhost:4000
