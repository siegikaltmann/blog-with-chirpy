---
title: "Kapitel 4 – Statik: Kräfte & Momente"
categories: [Physik, Statik]
tags: [kräfte, momente, gleichgewicht, fbd]
# layout/toc/math/mermaid kommen schon aus defaults
---

## 🎯 Lernziele
- Freikörperbild (FBD) erstellen.
- Gleichgewichtsbedingungen anwenden: $\sum F = 0$, $\sum M = 0$.
- Resultierende und Moment berechnen.

## 📘 Theorie
Momente: $$ M = F \cdot r $$  
Gleichgewicht: $ \sum F_x = 0,\ \sum F_y = 0,\ \sum M = 0$.

## 💻 Beispiel
```python
F, r = 500, 2.0
print("Moment =", F*r, "Nm")
