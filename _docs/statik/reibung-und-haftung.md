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
```

Ergebnis:
Normalkraft: 94.8 N
Haftreibung: 37.9 N
Gleitreibung: 28.4 N

🧠 Aufgabe
Ein 5 kg schwerer Block liegt auf horizontaler Fläche ($\mu_H = 0.5$, $\mu_G = 0.4$).
Welche Kraft ist nötig, um ihn gerade in Bewegung zu setzen?
✏️ Lösung:
$F_N = m \cdot g = 49.05,\mathrm{N}$
$F_R = \mu_H \cdot F_N = 24.5,\mathrm{N}$

🔍 Visualisierung (Mermaid)
graph TD
A[Körper] -->|F_G| B[Untergrund]
B -->|F_H| A

📘 Mermaid-Diagramme kannst du überall nutzen – Chirpy rendert sie automatisch.


