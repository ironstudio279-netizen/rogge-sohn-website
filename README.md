# Rogge & Sohn Elektrotechnik GmbH — Website

## Dateien
- `index.html` — Startseite (alles auf einer Seite)
- `impressum.html`, `datenschutz.html`, `cookie-richtlinie.html` — Rechtstexte (vor Veröffentlichung juristisch prüfen lassen)
- `404.html` — Fehlerseite
- `netlify.toml` / `vercel.json` — Hosting-Konfiguration
- `.nojekyll` — nötig für GitHub Pages, damit Dateien unverändert ausgeliefert werden

## Deployment

### Netlify (empfohlen, am einfachsten)
1. Auf netlify.com einloggen → „Add new site" → „Deploy manually"
2. Diesen gesamten Ordner per Drag & Drop hochladen
3. Fertig — Netlify erkennt `netlify.toml` automatisch (404-Seite, Security-Header)
4. Eigene Domain unter „Domain settings" verbinden, HTTPS wird automatisch aktiviert (Let's Encrypt)

### Vercel
1. Auf vercel.com einloggen → „Add New… → Project"
2. Diesen Ordner hochladen oder per GitHub-Repo verbinden
3. Vercel erkennt `vercel.json` automatisch
4. Domain verbinden, HTTPS automatisch aktiv

### GitHub Pages
1. Neues Repository erstellen, diesen Ordner hochladen (inkl. `.nojekyll`)
2. Repository-Einstellungen → „Pages" → Branch auswählen → Speichern
3. GitHub liefert automatisch HTTPS über `github.io`; eigene Domain optional über „Custom domain"
4. Hinweis: GitHub Pages unterstützt keine eigenen Server-Header — die Sicherheits-Header aus `netlify.toml`/`vercel.json` greifen hier nicht automatisch. Für volle Header-Kontrolle Netlify oder Vercel bevorzugen.

## Vor dem Live-Schalten unbedingt noch erledigen
Siehe Checkliste im Chat-Verlauf / letzte Chat-Antwort — Kurzfassung:
- [ ] Web3Forms Access Key im Kontaktformular eintragen (`index.html`, Suche nach "EINFÜGEN")
- [ ] Echte Fotos statt Platzhalter einsetzen (siehe `STOCK-PHOTOS.md`)
- [ ] Öffnungszeiten bestätigen und eintragen
- [ ] Rechtstexte (Impressum, Datenschutz) von einem Anwalt/Steuerberater prüfen lassen
- [ ] Analytics-Anbieter final festlegen (aktuell nur Platzhalter-Kommentar im Code)
- [ ] PageSpeed nach dem Livegang mit echten Bildern erneut mit Google PageSpeed Insights testen
