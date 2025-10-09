---
title: "Kapitel 4 – Statik: Kräfte & Momente"
date: 2025-10-09 09:00:00 +0200
categories: [Physik, Statik]
tags: [kräfte, momente, gleichgewicht, fbd]
math: true
mermaid: true
---

## 🎯 Lernziele
- Freikörperbild (FBD) erstellen.
- Gleichgewichtsbedingungen anwenden: $\sum F = 0$, $\sum M = 0$.
- Resultierende und Moment berechnen.

---

## 📘 Theorie

Eine **Kraft** $\vec F$ wird beschrieben durch:
- Betrag $F$ in Newton,
- Richtung (Winkel oder Komponenten),
- Angriffspunkt.

**Momente** entstehen durch Kräfte mit Abstand zum Bezugspunkt:
$$
M = F \cdot r
$$

**Gleichgewichtsbedingungen**:
$$
\sum F_x = 0, \quad \sum F_y = 0, \quad \sum M = 0
$$

---

## 💻 Beispiel

Ein Balken ist an einem Lager befestigt.  
Am Ende wirkt eine Kraft von $F = 500\,\mathrm{N}$ im Abstand $r = 2\,\mathrm{m}$.

Berechne das Moment:

```python
F = 500   # N
r = 2.0   # m
M = F * r
print(f"Moment = {M} Nm")
