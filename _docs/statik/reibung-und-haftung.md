---
title: "Kapitel 5 – Reibung & Haftung"
categories: [Physik, Statik]
tags: [reibung, haftung, gleiten]
---

## 🎯 Lernziele
- Unterschied zwischen **Haft-** und **Gleitreibung** verstehen  
- Reibungskraft berechnen  
- Zusammenhang zwischen Normalkraft und Reibkoeffizient erkennen

---

## 📘 Theorie

Die **Reibungskraft** $F_R$ ergibt sich aus der **Normalkraft** $F_N$ und dem **Reibungskoeffizienten** $\mu$:

$$
F_R = \mu \cdot F_N
$$

Es gilt:
- $\mu_H$ … Haftreibungskoeffizient  
- $\mu_G$ … Gleitreibungskoeffizient ($\mu_G < \mu_H$)

---

## 💻 Beispielrechnung

Ein Körper (Masse $m = 10\,\mathrm{kg}$) liegt auf einer schiefen Ebene ($\alpha = 15^\circ$).  
Gegeben: $\mu_H = 0.4$, $\mu_G = 0.3$.

```python
import math

m = 10        # kg
alpha = math.radians(15)
mu_H = 0.4
mu_G = 0.3
g = 9.81      # m/s²

F_N = m * g * math.cos(alpha)
F_H = mu_H * F_N
F_G = mu_G * F_N

print(f"Normalkraft: {F_N:.1f} N")
print(f"Haftreibung: {F_H:.1f} N")
print(f"Gleitreibung: {F_G:.1f} N")
