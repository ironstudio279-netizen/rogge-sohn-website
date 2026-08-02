# Bilder einsetzen: Anleitung

## Warum hier keine Bilder automatisch eingesetzt wurden
Bei der Suche nach "kostenlosen Elektriker-Bildern" liefern Bildersuchen meist Fotos von echten
anderen Elektro-Unternehmen (z. B. von deren Firmenwebsites) — das sind **keine** lizenzfreien
Stock-Fotos, sondern fremdes Bildmaterial mit Urheberrecht. Diese für Rogge & Sohn zu verwenden,
wäre eine Urheberrechtsverletzung. Deshalb bleiben die Platzhalter im Code bewusst als
Platzhalter markiert, statt automatisch (falsche) "lizenzfreie" Bilder einzusetzen.

## Empfohlene, garantiert lizenzfreie Quellen
- **Unsplash** (unsplash.com) — kostenlos, keine Attribution nötig
- **Pexels** (pexels.com) — kostenlos, keine Attribution nötig
- **Pixabay** (pixabay.com) — kostenlos, keine Attribution nötig

## Empfohlene Suchbegriffe
- "electrician" / "electrician at work"
- "fuse box" / "circuit breaker panel"
- "electrical wiring installation"
- "electrician tools"
- "modern office lighting"

## Wie die Bilder eingesetzt werden (pro Platzhalter im Code)
1. Bild bei Unsplash/Pexels/Pixabay herunterladen
2. **Umbenennen** in ein SEO-freundliches Format, z. B.:
   - `elektriker-verteilerschrank-berlin-spandau.jpg`
   - `elektroinstallation-altbau-spandau.jpg`
   - `lichtkonzept-buero-berlin.jpg`
3. **Komprimieren** vor dem Hochladen — z. B. mit [squoosh.app](https://squoosh.app) oder [tinypng.com](https://tinypng.com), Ziel: unter 150–200 KB pro Bild bei guter Qualität. Das ist der größte Hebel für Core Web Vitals (LCP).
4. Im Code den jeweiligen Platzhalter-`<div>` durch ein echtes `<img>`-Tag ersetzen, z. B.:
   ```html
   <img src="elektriker-verteilerschrank-berlin-spandau.jpg"
        alt="Elektriker montiert neuen Verteilerschrank in Berlin-Spandau"
        loading="lazy" decoding="async" width="600" height="600">
   ```
   `loading="lazy"` sorgt dafür, dass Bilder unterhalb des sichtbaren Bereichs erst bei Bedarf
   nachladen (bessere Ladezeit). `width`/`height` verhindern Layout-Sprünge (besserer CLS-Wert).
5. Format-Empfehlung: WebP statt JPG, wenn möglich (kleinere Dateigröße bei gleicher Qualität).

## Bessere Alternative
Sobald echte Fotos vom Betrieb selbst vorliegen (Team, Baustellen, Verteilerkästen), diese
anstelle von Stock-Fotos verwenden — das wirkt auf Kunden deutlich vertrauenswürdiger als
generische Stock-Bilder und ist für die Konversion i. d. R. wirkungsvoller.
