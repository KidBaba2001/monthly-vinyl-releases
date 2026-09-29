# Monthly Vinyl Releases

New house and techno vinyl releases from European record shops, grouped by shop, with previews and a cart.

## Files

- `index.html` – the whole page (design, player, filter, cart, glitch)
- `releases.json` – the release list. The daily update only changes this file.

## Publish with GitHub Pages

1. Create a new **public** repository on github.com, e.g. `monthly-vinyl-releases`.
2. Upload `index.html`, `releases.json` and this `README.md` (Add file → Upload files → Commit).
3. Settings → Pages → Source: *Deploy from a branch*, Branch: `main`, folder `/ (root)` → Save.
4. After a minute the page is live at `https://<your-username>.github.io/monthly-vinyl-releases/`.

## Daily update

Every morning a scheduled Claude task reads the shops' new-release pages, adds new records to `releases.json` and commits the file to this repository. GitHub Pages then publishes the new version automatically.

Shops that disallow automated reading (Deejay.de, oje-records.com) are not read.
