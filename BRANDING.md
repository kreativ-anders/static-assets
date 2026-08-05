# kreativ-anders Brand Guidelines

Quelle: `colors/style.css` (Referenz-Palette der `colors/index.html`-Vorschau).

## Farben

| Rolle       | Hex       |
|-------------|-----------|
| Akzent (Orange) | `#FFA500` |
| Schwarz (Text/Logo dark) | `#000000` |
| Weiß (Hintergrund/Logo light) | `#FFFFFF` |
| Dunkler Hintergrund | `#292929` |

Alle Logo-Dateien (SVG + PNG) und Share-Bilder in `logo/` und `images/` nutzen konsistent `#FFA500` als Akzentfarbe.

## Schrift

Oswald (400), eingebunden über `fonts/oswald-v47-latin-regular.woff2` / `.woff`, siehe `style.css`.

## Logo-Varianten (`logo/`)

- `dark.svg` / `dark-512.png` / `dark-large.png` / `dark-large.jpg` — dunkler Schriftzug, für helle Hintergründe.
- `light.svg` / `light-512.png` / `light.png` — heller (weißer) Schriftzug, für dunkle Hintergründe.
- `prefers-color-scheme.svg` / `prefers-color-scheme-font.svg` — passt Textfarbe automatisch per `prefers-color-scheme` an.

Alle Raster-Exporte teilen sich ein einheitliches Padding-Schema: quadratische Varianten (`-512`) sind 512×512 mit zentriertem Logo, großformatige Varianten folgen dem Seitenverhältnis von `dark-large.png` (~1.48:1).

## Verwendungshinweis

Dieses Repository wird als öffentliches Asset-CDN (`github.kreativ-anders.dev`) genutzt. Bestehende Dateipfade sollten nicht umbenannt oder verschoben werden, da sie extern verlinkt sein können.
