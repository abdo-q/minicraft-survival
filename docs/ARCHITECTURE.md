# Architecture

`index.html` is a single file. The main game module is an ES module whose header comment lists these sections (search for the word `SECTION`):

1. Vite helpers
2. Vendor: three.js r158 (do not edit)
3. Game: adaptive render distance
4. Vendor: howler.js 2.2.4 (do not edit)
5. Game: asset list, blocks, textures, mesher, player, physics, UI
6. Vendor: lil-gui 0.19.1 (do not edit)
7. Vendor: Comlink (worker RPC) (do not edit)
8. Game: biomes, terrain generation, World, Game class

Other parts of the file:
- A small script at the top manages the **worlds registry** in `localStorage` (`mc_worlds`, `mc_cur`).
- A `<script type="text/plain" id="worker-source">` block holds the Web Worker source that really generates terrain. The module also keeps a fallback copy, so **edit both** when changing terrain generation.
- `window.__ASSETS` holds base64-embedded textures, sounds and fonts.
- Additional inline scripts add UI features on top of the main module.
