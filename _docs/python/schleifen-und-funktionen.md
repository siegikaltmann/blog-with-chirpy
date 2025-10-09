---
title: "Python: Schleifen & Funktionen"
categories: [Informatik, Python]
tags: [programmierung, schleifen, funktionen]
---

## 🎯 Lernziele
- **for- und while-Schleifen** verstehen  
- **Funktionen** definieren und verwenden  

---

## 🔁 Schleifen

**for-Schleife:**
```python
for i in range(5):
    print("Iteration", i)
```

**while-Schleife**
```python
x = 0
while x < 5:
    print(x)
    x += 1
```

🧮 Funktionen
Eine Funktion wird mit def definiert:
def quadrat(x):
    return x * x

for i in range(1, 6):
    print(f"{i}² = {quadrat(i)}")
```

🧠 Aufgabe
Schreibe eine Funktion fakultaet(n), die die Fakultät einer Zahl berechnet.
Teste sie mit den Werten 3, 5 und 7.

✏️ Erwartete Ausgabe:
```
fak(3) = 6
fak(5) = 120
fak(7) = 5040
```




