---
title: "Gantt & Fortschritt"
project: diplomarbeit
layout: page
mermaid: true
permalink: /projekte/diplomarbeit/gantt/
---

```mermaid
gantt
  title Diplomarbeit 2025/26
  dateFormat  YYYY-MM-DD
  axisFormat  %d.%m.
  excludes    weekends

  section Planung
  Thema fixieren        :done,     t1, 2025-09-10, 2025-09-25
  Pflichtenheft         :active,   t2, 2025-09-26, 2025-10-15

  section Umsetzung
  Prototyp 1            :          m1, 2025-10-16, 2025-11-15
  Integration           :crit,     m2, 2025-11-16, 2025-12-20

  section Berichte
  Zwischenbericht 1     :milestone, z1, 2025-10-27, 0d
  Zwischenbericht 2     :milestone, z2, 2025-12-01, 0d
  Abgabe                :milestone, z3, 2026-02-28, 0d
```

