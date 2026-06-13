# 🌊 Rinmi — De Kalme Oceaan

Een kleurrijke, zijwaarts scrollende actie-/avonturengame met RPG- en
strategie-elementen, gebaseerd op het boek **"Rinmi"** (oorspronkelijke titel
*Dochters van de stilte*) van **Victoria Vermoolen**.

Speel als één van de vijf heldinnen, kies twee wapens, reis van het eiland met
de gevangenis, te paard naar Akuma's huis, door de donkere grotten, tot de
laatste strijd — en bevrijd Korea. En vergeet niet te eten: van honger ga je
dood!

> Alles zit in **één bestand**: `index.html`. Geen build, geen dependencies.

---

## ▶️ Spelen

- **Online:** zet het op GitHub Pages (zie hieronder) en open de link.
- **Lokaal:** open `index.html` in een moderne browser, of serveer de map:
  ```bash
  python3 -m http.server 8000
  # open daarna http://localhost:8000
  ```

### Besturing — toetsenbord
| Toets | Actie |
|---|---|
| ← → / A D | Lopen |
| ↑ / W / Spatie | Springen (Qingfei: ingedrukt houden = zweven) |
| X / J | Aanvallen |
| C / K | Wapen wisselen |
| S / Shift | Je gave (elke heldin een andere!) |
| 1 · 2 · 3 | Eten · drinken · levensmiddel |
| Tab | Tas & statistieken |
| P / Esc | Pauze |

### Besturing — touch (iPhone/iPad/Android) 📱
Native touchbediening, geen virtuele D-pad:
- **Linkerhelft = zwevende joystick** — leg je duim neer en sleep om te lopen
  (en omhoog/omlaag om te zwemmen met Rinmi).
- **Rechterhelft = gebaren:**
  - **Tik** = aanvallen
  - **Veeg omhoog** = springen (vinger omhoog houden = zweven met Qingfei)
  - **Veeg omlaag** = je gave
- **Knoppen onderin:** 🍙 eten · 💧 drinken · ✚ levensmiddel · ✦ gave · wapen · ⏸ pauze.

Speel liggend (landscape). Tip: voeg de pagina toe aan je beginscherm
("Zet op beginscherm") om Rinmi schermvullend als app te spelen.

---

## 🚀 Deployen met GitHub Pages

### Optie A — kant-en-klaar (aanbevolen)
1. Maak een nieuwe GitHub-repository en push deze map (met `index.html` in de
   hoofdmap).
2. Ga naar **Settings → Pages**.
3. Bij **Build and deployment → Source** kies je **GitHub Actions**.
4. De meegeleverde workflow (`.github/workflows/pages.yml`) publiceert de site
   automatisch bij elke push naar `main`. Je link verschijnt onder *Settings →
   Pages*.

### Optie B — zonder Actions
1. Push de map naar GitHub.
2. **Settings → Pages → Source: Deploy from a branch**.
3. Kies branch `main` en map `/ (root)`. Klaar — `index.html` wordt direct
   geserveerd. (`.nojekyll` zorgt dat alles ongewijzigd wordt geserveerd.)

```bash
# Snel een repo opzetten en pushen:
git init -b main
git add .
git commit -m "Rinmi — De Kalme Oceaan"
git remote add origin https://github.com/<jouw-naam>/<repo>.git
git push -u origin main
```

---

## 🎮 Wat zit erin
- **5 speelbare heldinnen**, elk met een eigen gave: Rinmi (water geneest haar,
  zwemmen, genezende watergolf), Kana (rode bliksem-dash), Yuna (valstrikken),
  Qingfei (zweven + windvlaag), Seojin (rotsen verplaatsen).
- **2 wapens kiezen** uit zwaard, pijl & boog, zwaaibanden en katapult.
- **RPG:** XP, niveaus, statpunten (Kracht/Vitaliteit/Snelheid), oma's winkel,
  mun-munten, levens, highscore.
- **Overleving:** hongermeter — eet op tijd! — water, etenspakketten,
  levensmiddel.
- **Reis door 3 levels + proloog + paardrit + eindbaas Akuma.**
- Boordevol grapjes en verwijzingen naar het boek. 🌸

## Credits
Verhaal: **Victoria Vermoolen** (*Dochters van de stilte*).
Nagekeken door Koos van Starrenburg. Opgedragen aan Joanne Plattel.
Spel gebouwd met canvas + vanilla JavaScript.
