# Identité visuelle — coulon-deville.dev

## `logos-complets/`

Icône + `coulon-deville.dev` + « Florent Coulon-Deville ». Texte vectorisé, aucune police requise.

| Fichier | Icône |
|---|---|
| `logo-cd-*` | Monogramme CD |
| `logo-prompt-*` | Prompt `>_` |
| `logo-prompt-cd-*` | Prompt `> cd` |

Chaque logo existe en `-clair` (pour fond clair) et `-sombre` (pour fond sombre), en `.svg`, `@2x.png` et `@4x.png`.

## `icones/`

| Dossier | Icône |
|---|---|
| `cd/` | Monogramme CD |
| `prompt/` | Prompt `>_` |
| `prompt-cd/` | `> cd` |
| `cd-curseur/` | `cd_` |

Fichiers de chaque dossier :

| Fichier | Usage |
|---|---|
| `icon.svg` / `icon-512.png` / `icon-1024.png` | Icône principale (carré arrondi) |
| `favicon.svg` / `favicon.ico` (16-32-48) | Favicon (traits épaissis) |
| `apple-touch-icon.png` (180) | iOS |
| `manifest-192.png` / `manifest-512.png` | Web manifest |
| `avatar-github.svg` / `avatar-github-500.png` | Avatar GitHub (recadrage rond) |
| `glyph.svg` / `glyph-1200.png` | Logo seul, fond transparent, pour fond clair |
| `glyph-blanc.svg` / `glyph-blanc-1200.png` | Logo seul, fond transparent, pour fond sombre |

Polices : Space Grotesk Bold (nom) · JetBrains Mono Medium (sous-titre), licence SIL OFL.
Couleurs : bleu nuit `#1B2559` · bleu nuit clair `#2A3775` · blanc `#FFFFFF` · accent `#FF8A3D`

## Intégration HTML (GitHub Pages)

Copier les fichiers de l'icône choisie à la racine du site.

```html
<link rel="icon" href="/favicon.ico" sizes="any">
<link rel="icon" href="/favicon.svg" type="image/svg+xml">
<link rel="apple-touch-icon" href="/apple-touch-icon.png">
<link rel="manifest" href="/site.webmanifest">
```

`site.webmanifest` :

```json
{
  "name": "coulon-deville.dev",
  "short_name": "coulon-deville",
  "icons": [
    { "src": "/manifest-192.png", "sizes": "192x192", "type": "image/png" },
    { "src": "/manifest-512.png", "sizes": "512x512", "type": "image/png" }
  ],
  "theme_color": "#1B2559",
  "background_color": "#1B2559",
  "display": "standalone"
}
```
