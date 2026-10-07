# kreativ-anders Brand Guidelines

Quelle: `colors/style.css` (Referenz-Palette der `colors/index.html`-Vorschau).

## Farben

| Rolle       | Hex       |
|-------------|-----------|
| Akzent (Orange) | `#FFA500` |
| Schwarz (Text/Logo dark) | `#000000` |
| Weiß (Hintergrund/Logo light) | `#FFFFFF` |
| Dunkler Hintergrund | `#292929` |

Blau und Gelb (Ukraine-Solidarität, 2022–2026) werden nicht mehr verwendet, siehe `archive/`. Auf der Website gilt:
Orange als einzige Akzentfarbe, dazu Hell/Dunkel und Abstufungen des Orange (z. B. `#C66A00` für den Trend-Strich in
`animations/success.svg`).

Alle Logo-Dateien (SVG + PNG) und Share-Bilder in `logo/` und `images/` nutzen konsistent `#FFA500` als Akzentfarbe.

## Schrift

Oswald (400), eingebunden über `fonts/oswald-v47-latin-regular.woff2` / `.woff`, siehe `style.css`.

## Logo-Varianten (`logo/`)

- `logo.svg` — **Standard.** Schriftzug passt sich Hell/Dunkel an (`light-dark()`, Fallback `prefers-color-scheme`),
  Oswald ist als WOFF2-Subset (nur die Buchstaben des Logos, ~1 KB) eingebettet – keine externe Schrift nötig.
- `logo-outlined.svg` — wie `logo.svg`, Schriftzug als Pfade (für Favicon, Grafikprogramme, Druck).
- `dark.svg` / `dark-512.png` / `dark-large.png` / `dark-large.jpg` — dunkler Schriftzug, für helle Hintergründe.
- `light.svg` / `light-512.png` / `light.png` — heller (weißer) Schriftzug, für dunkle Hintergründe.
- `prefers-color-scheme.svg` / `prefers-color-scheme-font.svg` — frühere Namen des adaptiven Logos, identisch mit
  `logo.svg` (die Hell/Dunkel-Logik war vertauscht und ist korrigiert).

Alle SVGs betten die Schrift ein; Google Fonts wird nicht mehr geladen. `favicon.svg` entspricht `logo-outlined.svg`.

Ein als `<img>` eingebundenes SVG folgt der Systemeinstellung, nicht einem Theme-Umschalter der Seite. Wo die Seite das
Farbschema selbst umschaltet, das Logo inline einbinden (siehe `layouts/_partials/logo.html` in ideenfabrik).

## Animationen (`animations/`)

`lean.svg`, `transparent.svg`, `success.svg` (400×400, je unter 1 KB) ersetzen die GIFs der Startseite (zusammen 44 KB).
Der Logo-Rahmen wird gezeichnet, gehalten und wieder ausgeblendet (5-Sekunden-Loop). Das CSS steckt im SVG; bei
„Bewegung reduzieren“ erscheint das Standbild. Vorschau: `animations/index.html`.

## Archiv (`archive/`)

- `ukraine-solidarity/` — blau-gelbes Logo der Website (bis Oktober 2026). Nicht mehr verwenden.

Alle Raster-Exporte teilen sich ein einheitliches Padding-Schema: quadratische Varianten (`-512`) sind 512×512 mit zentriertem Logo, großformatige Varianten folgen dem Seitenverhältnis von `dark-large.png` (~1.48:1).

## Verwendungshinweis

Dieses Repository wird als öffentliches Asset-CDN (`github.kreativ-anders.dev`) genutzt. Bestehende Dateipfade sollten nicht umbenannt oder verschoben werden, da sie extern verlinkt sein können.
