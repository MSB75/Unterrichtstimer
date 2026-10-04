# Unterrichtstimer – Offline-PWA

## Dateien
- `index.html` – vollständige App
- `manifest.webmanifest` – PWA-Metadaten
- `sw.js` – Offline-Cache
- `icons/` – App-Symbole

## Funktionen
- analoge Uhr mit aktueller Uhrzeit
- Unterrichtsphasen als Segmente um die Uhr
- Start, Pause, Stop und Ausblenden der Phasen
- optionale Startverzögerung in Minuten
- Tonsignale: Schulgong, Digital, Sanft, Stumm
- Timer hinzufügen und löschen
- optionale lokale Bilder pro Timerphase
- Vollbild bzw. kompakte Ansicht
- Infobereich mit Datenschutz- und Kontaktangaben
- Offline-PWA

## Bereitstellung
Alle Dateien gemeinsam auf einen HTTPS-Webspace oder in ein GitHub-Pages-Repository hochladen. Danach die `index.html` in Safari öffnen und über „Teilen“ → „Zum Home-Bildschirm“ installieren.

## Hinweise
Die ausgewählten Bilder werden lokal im Browser gespeichert. Für sehr große Bilder ist eine Dateigröße unter 2,5 MB vorgesehen.


## Version 1.1
- Unterrichtsphasen werden minutengenau in Bezug auf die reale Uhrzeit als farbige Segmente dargestellt.
- Die aktive Phase schrumpft mit dem laufenden Minutenzeiger.
- Start- und Endminute jeder Phase werden an der Uhr angezeigt.
- Lokale Bilder/Icons der Phasen erscheinen zusätzlich auf den Farbsegmenten.
- Phasenbezeichnungen rechts verwenden dieselben Farben.
- Sekundenzeiger läuft flüssig über `requestAnimationFrame`.
- Digitale Uhrzeit und verbleibende Zeit wurden aus dem Inneren der analogen Uhr entfernt.


## Version 1.2
- Schülernamen können in der Timerkonfiguration hinterlegt werden.
- Pro Unterrichtsphase kann die Mitarbeit je Schüler über Rot/Gelb/Grün bewertet werden.
- Aus den Bewertungen wird eine Rangfolge mit Gold, Silber und Bronze erstellt.
- Minuten-Zahlen an den Beginn-/Endpunkten der Farbfelder wurden entfernt.
- Die Phasenkarten rechts wurden grafisch klarer und sauberer gerahmt.
- Die Phasenanzeige unterhalb der Uhr wurde kompakter zwischen die unteren Bedienelemente gesetzt.


## Version 1.3
- Farbliche Markierungen am Uhrenrand sind voll deckend und einheitlich breit.
- Bewertungs- und Platzierungsbereiche wurden deutlich kompakter gestaltet.
- Alle Unterrichtsphasen sollen gleichzeitig auf der rechten Seite sichtbar bleiben.
- Scrollbedarf wurde weiter reduziert.
- Neue Stunden-Presets für 45, 60 und 90 Minuten.
- Zehn Schnell-Icons für Unterrichtsphasen: 👋 ✏️ 📖 🧠 👥 💬 🎯 ✅ 🧹 🎨.
- Eigene Bilder können weiterhin zusätzlich verwendet werden.


## Version 1.4
- Stundenlängen-Presets wurden entfernt.
- Zehn Schnellbilder können frei aus lokalen Ordnern belegt werden.
- Schnellbilder lassen sich jeder Unterrichtsphase direkt zuordnen.
- Die laufende Timerphase bleibt auf dem äußersten Farbring sichtbar.
- Später liegende Timer werden auf weiter innen liegenden Ringbahnen dargestellt.
- Dadurch überlagern spätere Phasen die laufende Visualisierung nicht mehr.


## Version 1.5
- Individuelle Unterrichtsziele können pro Schüler angelegt werden.
- Jedes Ziel kann mit einem selbst ausgewählten lokalen Bild visualisiert werden.
- Die Ampelbewertung erfolgt pro Unterrichtsphase und pro individuellem Ziel.
- Die abschließende Schülerplatzierung wird aus den Zielbewertungen zusammengefasst.


## Version 1.6
- Schnellbilder, Schülernamen und individuelle Unterrichtsziele sind in der Konfiguration einklappbar.
- Eigene Schulstunden können unter frei wählbaren Namen gespeichert werden.
- Gespeicherte Stunden enthalten die jeweilige Phasenübersicht mit Reihenfolge, Dauer und Bildern.
- Zwischen z. B. Mathe- und Deutschstunden kann direkt gewechselt werden.
- Schülernamen und individuelle Unterrichtsziele bleiben unabhängig von den gespeicherten Stunden erhalten.


## Version 1.7
- Schnellbilder von 10 auf 20 frei belegbare Bildplätze erweitert.
- Bestehende gespeicherte Schnellbilder werden übernommen; zusätzliche Plätze bleiben zunächst leer.
