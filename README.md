# Endless Labyrinth

**[Play Endless Labyrinth](https://bimmerman1911.github.io/Endless-Labyrinth/)**

A browser-based 2D maze game. Search wooden drawers for a hidden key, unlock the green exit, and descend through an endless series of randomly generated floors.

Inspired by the story: “I spelet ska det finnas byrålådor där man kan hitta en nyckel. De kan vara i trä.”

## Play

Open **index.html** directly in a current browser. No installation, build, account, or backend is required. An optional Google Fonts stylesheet improves typography; system fonts are used when offline.

- **Move:** WASD or arrow keys; directional buttons on phones and touch devices.
- **Search:** E, Space, or the Search button while standing on or beside a drawer. You can also click or tap an adjacent drawer.
- **Escape:** Collect the key, then reach the green exit before your 3-minute lantern runs out.
- **Continue:** The next floor has a fresh maze and lantern. Your score carries over.
- **Pause:** P, Escape, or Pause. Leaving the tab pauses automatically.
- **Restart:** Restart returns to the start screen with a new maze and zero score.
- **Sound:** Optional synthesized sounds, muted by default.

Search a drawer for **25 points**, find the key for **100 extra points**, and escape for **250 points plus twice the number of remaining seconds**. Your personal best stays on the device when browser storage is available.

## Publish in your existing GitHub repository

1. Upload `index.html`, `style.css`, `game.js`, and `.nojekyll` to the **root** of your `Endless-Labyrinth` repository. Include this README if desired. Do not place them inside an extra folder.
2. Commit the files to `main` (or your chosen default branch).
3. Open **Settings → Pages** in the repository.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select **main** and **/ (root)**, then save.
6. Wait for the Pages deployment to finish. GitHub displays the live link under Settings → Pages.

For a standard project repository, the URL will be:

https://bimmerman1911.github.io/Endless-Labyrinth/

All game assets use relative paths, so hosting under the repository subpath works. GitHub Pages must be enabled on an account/repository plan that supports public publishing.

## Files

- `index.html` — entry point, interface, start screen, instructions.
- `style.css` — responsive styling and touch controls.
- `game.js` — procedural maze generation, canvas rendering, controls, scoring, local best score, synthesized audio.
- `.nojekyll` — tells GitHub Pages to serve the static files directly.

## Verification

JavaScript syntax checked with Node. A headless logic harness verified connectivity and key placement across 100 generated mazes, locked exits, key collection, scoring, next-floor progression, pause/resume, touch event handling, timeout, restart, and personal-best persistence. Browser visual QA was unavailable in the build environment, so check the published game on your target desktop and phone browsers.
