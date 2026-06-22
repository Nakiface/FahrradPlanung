# Rennrad-Basislager Europa — Astro-Website

Interaktive Übersicht der zehn Basislager mit Menüleiste, Top-Anstiegen (Höhe, Länge, Höhenmeter, Ø-/Max-Steigung) und selbst erzeugten SVG-Höhenprofilen.

## Fertige Seite ansehen

Einfach `dist/index.html` per Doppelklick im Browser öffnen — die Seite ist self-contained (alle Styles, Skripte und Grafiken inline), es ist kein Server nötig.

## Selbst bearbeiten / neu bauen

Voraussetzung: Node.js 18.17+ (entwickelt mit Node 22).

```bash
npm install
npm run dev      # lokaler Entwicklungsserver
npm run build    # erzeugt dist/index.html
```

Alle Inhalte (Orte, Anstiege, Werte) stehen als Datenarray oben in `src/pages/index.astro` — dort lassen sich Werte ergänzen oder korrigieren, danach `npm run build`.

## Hinweis zu den Werten

Höhen, Längen und Höhenmeter sind gängige Richtwerte (Stand Juni 2026). Die Ø-Steigung wird aus Höhenmeter/Länge berechnet; Max-Steigungen sind mit „ca." gekennzeichnete Näherungen. Die Höhenprofile sind stilisierte Darstellungen des Gesamtanstiegs, keine vermessenen GPX-Profile.
