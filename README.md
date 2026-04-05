[README.md](https://github.com/user-attachments/files/26486942/README.md)
# 🐧 Breatheflow 1.0.3

> Učíme tě dýchat — od základů až po pokročilá dechová cvičení.

Breatheflow je seversky inspirovaná webová aplikace pro dechová cvičení. Bez instalace, bez přihlašování — stačí otevřít v prohlížeči.

---

## ✨ Funkce

- **Maximální výdrž** — zadrž dech, tučňák se potápí a zobrazuje hloubku v metrech (vychází z rychlosti tučňáka 8 km/h = 2,222 m/s)
- **Větší přítomnost** — Box Breathing technika 4-4-4-4
- **Práce se stresem** — 4-7-8 technika Dr. Weila
- **Osobní profil** — localStorage, žádný backend
- **Graf výdrže** — SVG line chart přes dny
- **Globální žebříček** — seeded leaderboard
- **Tučňákovy funfacts** po každém cvičení
- **Zvukový engine** — Web Audio API, fázové tóny
- **Severský design** — glassmorphism, oceánová paleta, animované bubliny

---

## 🚀 Spuštění

Žádné závislosti, žádný build step:

```bash
git clone https://github.com/твой-username/breatheflow.git
cd breatheflow
# Otevři index.html v prohlížeči nebo spusť lokální server:
npx serve .
# nebo:
python3 -m http.server 8080
```

---

## 📁 Struktura

```
breatheflow/
└── index.html   # Celá aplikace — HTML + CSS + JS v jednom souboru
```

---

## 🗂 localStorage klíče

| Klíč | Obsah |
|------|-------|
| `bf_profile` | `{ nick, age, gender }` |
| `bf_history` | Pole lekcí `{ type, time, date, name }` |
| `bf_lessons` | Počítadla `{ hold, pres, str }` |

---

## 🐧 O tučňákovi

Tučňák plave rychlostí **8 km/h (2,222 m/s)**. Hloubka ponoru se počítá jako:

```
hloubka (m) = čas_výdrže (s) × 2.222
```

Císařský tučňák se dokáže ponořit až **500 m** a zadržet dech **22 minut** — ty to zkus překonat!

---

## 👤 Autor

**Michal Soulak**

---

