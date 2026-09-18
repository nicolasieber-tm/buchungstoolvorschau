# Buchungstool – Admin-Backend (Vorschau)

Einfache HTML-Vorschau für das Verwaltungs-Backend: Dashboard, Termine/Buchungen,
Angebote & Preise, Kalender-Verbindung (Angebot → Unterkalender, Verfügbarkeit) sowie eine
Website-Vorschau: Demo-Website mit Buchungs-Overlay aus Kundensicht. Das Overlay zeigt die
aktiven Angebote und sperrt Zeiten, die im Planer belegt sind; Testbuchungen landen im Planer.

Reine Vorschau/Referenz – keine echte Datenspeicherung, keine echte Kalender-Anbindung.
Buttons zeigen Demo-Meldungen.

## Lokal starten

```bash
npm start
# -> http://localhost:3000
```

(Node 18+ nötig, keine Abhängigkeiten zu installieren.)

## Deployment auf Railway

1. Repo auf GitHub pushen.
2. Railway: **New Project → Deploy from GitHub repo** und dieses Repo wählen.
3. Railway erkennt Node automatisch und führt `npm start` aus (Server bindet an `$PORT`).
4. **Settings → Networking → Generate Domain** für eine öffentliche URL.

## Dateien

- `index.html` – komplette Admin-Vorschau (HTML/CSS/JS in einer Datei)
- `server.js` – minimaler statischer Webserver (zero-dependency)
- `package.json` – Start-Skript
