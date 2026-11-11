# Simple Mind Map

A mind-map tool that runs entirely in your browser. One HTML file, no build step, works offline, installs as an app.

## Features
- Outline pane, level filter (1-4 / All), search, collapse, focus branch, tag filter
- Mouse and touch: pan, wheel/pinch zoom, drag nodes to re-parent, long-press menu
- Undo/redo, notes, tags, colors, due date, priority, tasks, two layouts
- Version history (automatic snapshots, named versions, restore) and zip backup/restore
- Export: FreeMind `.mm`, OPML, Markdown, draw.io, SVG, PNG, native JSON. Import the same, or paste an indented list
- Storage: this device (IndexedDB) and optional Dropbox sync. Google Drive is not built yet.

## Host on GitHub Pages
1. Push these files to the repo root.
2. Settings > Pages > Deploy from branch > `main` / root.
3. Open `https://<user>.github.io/simple-mind-map/`.

## Dropbox sync
1. Create an app at https://www.dropbox.com/developers/apps (Scoped access, App folder).
2. Permissions: `files.content.read` and `files.content.write`.
3. Add your Pages URL (exactly, e.g. `https://<user>.github.io/simple-mind-map/`) as a Redirect URI.
4. In the app: Settings, paste the App key, then Connect.

Conflicts keep both: your local version stays and the Dropbox one is saved as "(Dropbox copy)".

## Updating
Bump `VERSION` in `sw.js` after each change so installed copies refresh.

## Shortcuts
Press `?` in the app. Ctrl+K opens the command palette.
