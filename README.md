# Betonfiguren Preisliste

Preisliste für handgefertigte Betonfiguren -- Ostermarkt Edition.

**Live:** [andygubser.github.io/handwerk-mit-herz](https://andygubser.github.io/handwerk-mit-herz/)

## Dateien

| Datei | Beschreibung |
|-------|-------------|
| `index.html` | Interaktive Preisliste (Kartenansicht mit Lightbox) |
| `print.html` | Druckoptimierte Kartenansicht (2 Seiten A4) |
| `tabelle.html` | Tabellarische Preisliste mit Miniaturbildern |

## Datenquelle

Alle Produkte werden aus `prices/prices.json` geladen. Die HTML-Dateien enthalten eine eingebettete Kopie als Fallback.

## Struktur

```
├── index.html              Hauptseite (Web)
├── print.html              Druckversion (Karten)
├── tabelle.html            Druckversion (Tabelle)
├── prices/
│   └── prices.json         Produktdaten (Name, Preis, Bilder)
├── images/
│   ├── *.png / *.jpg       Aktive Produktbilder
│   ├── logo.jpg            Logo
│   ├── archive/            Ältere Produktfotos (nicht im Repo)
│   └── heic-converted/     Konvertierte HEIC-Dateien (nicht im Repo)
└── .github/workflows/
    └── pages.yml           GitHub Pages Deployment
```

## Deployment

Pusht automatisch via GitHub Actions auf GitHub Pages bei jedem Push auf `main`.
