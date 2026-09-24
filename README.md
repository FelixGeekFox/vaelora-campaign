# Vaelora Campaign Portal

A responsive, single-page campaign portal for **Vaelora**, Kris's dark fairy-tale Dungeons & Dragons campaign.

> The gods are silent. The old promises are not.

## Local preview

The site has no build step or package dependencies. Open `index.html` directly, or run a small local server:

```powershell
python -m http.server 4173
```

Then visit <http://localhost:4173>.

## Editing the site

- Campaign copy and page sections live in `index.html`.
- Colours, typography, layout, and the illustrated hero live in `styles.css`.
- Navigation and reveal effects live in `script.js`.
- The bell emblem is `assets/vaelora-mark.svg` and the regional map is `assets/vaelora-map.jpg`.

Search for the section heading you want to change. Each section has a readable ID:

| ID | Section |
| --- | --- |
| `premise` | The campaign premise and the Great Hush |
| `wyrd` | The Wyrd, and the five things everyone knows |
| `wickhollow` | Wickhollow and the seventh bell |
| `customs` | Everyday customs, wards, and contradictions |
| `knowledge` | Common knowledge, and what each background knows |
| `regions` | The four regions of Vaelora |
| `map` | The illustrated map |
| `peoples` | Peoples of Vaelora and living with difference |
| `questions` | Prompts for magical or unusual characters |
| `magic` | Arcane, innate, divine, primal, and pacts |
| `characters` | Creation defaults, concept, species, and classes |
| `connections` | Starting connections and ties to the world |
| `rumours` | The sixteen rumours and old cautions |
| `table` | Cooperative play, DM authority, safety and boundaries |
| `checklist` | The before-session-one checklist |
| `chronicle` | Session records (empty until play begins) |

### Replacing the map

`assets/vaelora-map.jpg` is a 1536x1024 JPEG. Swap in a new file at the same path, and update the `width`, `height`, and `alt` attributes on the image in the `map` section if the dimensions change.

## Adding the player PDF

When the campaign packet is ready:

1. Create a `downloads` folder.
2. Add the PDF as `downloads/vaelora-player-guide.pdf`.
3. Add or update a link in `index.html`:

```html
<a href="downloads/vaelora-player-guide.pdf">Download the player guide</a>
```

## Publishing

This repository is designed for GitHub Pages. Publish from the `main` branch and repository root.

## Canon

Kris is the final authority on campaign canon and table rulings. Public material should remain player-safe and should not include unrevealed DM information.
