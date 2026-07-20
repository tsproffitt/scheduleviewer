# Faculty Schedule Viewer — deploy site

Public, git-linked Netlify site. **`index.html` is generated** — do not edit it here.

- Source of truth: `../Schedule Viewer/` (template + `Master Schedule - Fall 2026.xlsx`).
- To update: run `python3 refresh.py --deploy` from `../Schedule Viewer/`.
  That rebuilds the viewer, copies the **faculty** build into `index.html`, commits, and pushes.
  Netlify auto-publishes on push (~30s).
- The **admin** build (teaching/room minutes) is deliberately NOT in this repo — it stays local.

Only the faculty file, `netlify.toml`, `robots.txt`, and this README live here.
