# @sero-ai/plugin-tetris

Classic Tetris game for Sero — a full-featured arcade game with HD particle
effects, smooth animations, and responsive controls.

## Sero Plugin Install

Install in **Sero → Admin → Plugins** with:

```text
git:https://github.com/monobyte/sero-tetris-plugin.git
```

Sero clones the source repo, installs its dependencies locally, builds the UI,
and then hot-loads the plugin into the sidebar.

## Pi CLI Usage

Install as a Pi package:

```bash
pi install git:https://github.com/monobyte/sero-tetris-plugin.git
```

Tetris is a UI-only app — it registers a minimal extension with no agent tools.
The game runs entirely in the browser.

## Sero Usage

When loaded in Sero, the Tetris game mounts in the main app area. Use keyboard
controls to play:

- **← / →** — Move piece left / right
- **↑** — Rotate piece
- **↓** — Soft drop
- **Space** — Hard drop

## Development

```bash
npm install
npm run dev          # Start Vite dev server
npm run build        # Production build → dist/ui/
npm run typecheck    # Type-check the UI code
```

## Build Output

```
dist/ui/
├── remoteEntry.js      # Module Federation remote entry
├── mf-manifest.json    # Federation manifest
└── assets/             # Chunks and CSS
```
