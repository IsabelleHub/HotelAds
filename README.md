# Panther Consulting – Hospitality Landingpage

Statische Seite (HTML/CSS/JS, kein Build-Schritt nötig) für die Hotel-Sparte von Panther Consulting.

## Struktur
- `index.html` – Seiteninhalt
- `styles.css` – Design
- `script.js` – Mobile-Navigation, Footer-Jahr
- `vercel.json` – kleine Konfiguration (saubere URLs)

## Deploy auf Vercel

**Option A – ohne GitHub (am schnellsten):**
1. [vercel.com](https://vercel.com) → Account/Login
2. „Add New… → Project“ → „Deploy“ ohne Git-Repo, stattdessen Ordner per Drag & Drop hochladen (die drei Dateien + `vercel.json`)
3. Vercel erkennt es automatisch als statische Seite – kein Framework auswählen nötig

**Option B – über GitHub (empfohlen für spätere Änderungen):**
1. Diesen Ordner in ein neues GitHub-Repo pushen
2. Auf [vercel.com](https://vercel.com) → „Add New… → Project“ → Repo auswählen
3. Framework Preset: „Other“ / „Static“ lassen, Deploy klicken

**Option C – Vercel CLI:**
```bash
npm i -g vercel
cd panther-hospitality-site
vercel
```

## Offene Punkte vor dem Live-Schalten
- `mailto:hello@pantherconsulting.com` im Kontakt-CTA auf deine echte Adresse anpassen
- Impressum/Datenschutz-Links im Footer sind Platzhalter (`#`) – rechtssicheren Text ergänzen
- Referenz-Sektion verlinkt aktuell nicht auf einen Case – ggf. Link zu venue-packages.com oder einem Mini-Case ergänzen
- Domain in Vercel-Projekteinstellungen verbinden, sobald du dich für Subdomain vs. eigene Domain entschieden hast
