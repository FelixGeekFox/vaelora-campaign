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
- The bell emblem is `assets/vaelora-mark.svg`.

Search for the section heading you want to change. Each major section has a readable ID such as `premise`, `regions`, `characters`, or `chronicle`.

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
