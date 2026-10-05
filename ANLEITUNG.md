# Sakura & Jade WorkFlow – Installation

Die App ist eine PWA: Sie läuft komplett offline, speichert alles im Gerätespeicher (IndexedDB) und lässt sich wie eine App installieren.

## Variante A – Schnell testen (Laptop)
    cd sakura-jade
    python -m http.server 8080
Dann http://localhost:8080 im Chrome/Edge öffnen. In der Adressleiste erscheint „Installieren“.

## Variante B – Aufs Handy (empfohlen)
1. Den Ordner kostenlos hosten (GitHub Pages, Netlify Drop oder Cloudflare Pages – einfach den Ordner hochladen).
2. Die Adresse einmal am Handy öffnen (HTTPS nötig, nur für den ersten Aufruf).
3. iPhone: Safari -> Teilen -> „Zum Home-Bildschirm“. Android: Chrome -> Menü -> „App installieren“.
Danach funktioniert alles ohne Internet. Die Daten bleiben auf dem Gerät.

## Backups
Einstellungen -> Backup (.json) exportieren / teilen / importieren (Zusammenführen für Handy <-> Laptop).
Zusätzlich legt die App automatisch Tages-Sicherungen der letzten 3 Tage im Gerätespeicher an.

## Dateien
index.html, style.css, app.js, wushu-data.js – App
sw.js, manifest.webmanifest – Offline & Installation
fonts/, icons/ – Schrift und Symbole
