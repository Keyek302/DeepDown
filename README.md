# Deep Down

An idle dungeon crawler for phones. Build a party of six heroes, fight down through five zones and 40 monsters, collect relics and pets, then retire the party for soul shards and go deeper.

Everything is in `index.html`: no build step, no libraries, and all sound is generated in the browser.

## Files

- `index.html` — the whole game
- `manifest.webmanifest` — app name, colours and icons for installing
- `sw.js` — service worker that lets the game run offline
- `icons/` — app icons (192, 512 and the 180 px Apple touch icon)

## Put it on GitHub Pages

1. Create a new repository, for example `DeepDown`.
2. Upload every file in this folder, keeping `icons/` as a folder.
3. In the repository, open Settings, then Pages, and set the source to the `main` branch, root folder.
4. After a minute the game is live at `https://<your-username>.github.io/DeepDown/`.

## Install it as an app

- Android (Chrome): open the link and tap "Install as an app" on the title screen, or use the browser menu, then "Add to Home screen".
- iPhone (Safari): open the link, tap Share, then "Add to Home Screen".

Once installed and opened online one time, it works offline.

## Updating

Upload the new `index.html`. If you also change icons or the manifest, bump `CACHE` in `sw.js` (for example to `deep-down-v2`).

Saves are kept in the browser on each device. Clearing site data erases them.
