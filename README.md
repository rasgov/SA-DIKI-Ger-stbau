# SA-DIKI Gerüst & Bau – Website

## Struktur
```
index.html              Seite (Three.js + GSAP per CDN, Tailwind lokal)
assets/css/style.css    fertig gebautes Tailwind-CSS (produktionsbereit)
assets/img/             Logo-Emblem, Logos, Favicons
src/input.css           Tailwind-Quelle (Farben, Schriften, eigene Komponenten)
package.json            Build-Skripte
```

## Hochladen
`index.html` und den Ordner `assets/` auf den Webserver laden (beide nebeneinander).
`src/`, `package.json` und `README.md` werden nur für Änderungen am CSS gebraucht.

## CSS neu bauen (nach Änderungen an Klassen in index.html oder an src/input.css)
Voraussetzung: Node.js 20+

```bash
npm install
npm run build     # einmalig, minifiziert
npm run watch     # während der Entwicklung
```

Offizielle Anleitung: https://tailwindcss.com/docs/installation/tailwind-cli
