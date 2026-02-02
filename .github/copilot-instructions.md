# Copilot / AI Agent Instructions for this repo

This repository is a very small, static web project. The goal of these instructions is to help AI coding agents be immediately productive and avoid generic advice.

1. Big picture
- Single-page static website: the app entry is `webantoanmang2.html` at the repo root. There is no build system, package manager, or server-side code.
- Primary intent: static HTML/CSS (possibly Vietnamese content). Changes are typically edits to the single HTML file or adding static assets.

2. Key files and examples
- `webantoanmang2.html`: main and only application file. Inspect this first for structure, inline scripts, or references to assets.
- `.gitattributes`: small repo metadata; no build info.

3. Developer workflows (concrete commands)
- Preview locally (recommended): run a simple HTTP server from the repo root:
  - `python -m http.server 8000` (then open http://localhost:8000/webantoanmang2.html)
  - or use VS Code Live Server to serve the file.
- No test runner or build steps present — avoid adding build tooling unless requested by a maintainer.

4. Project conventions (discoverable patterns)
- Keep edits minimal and focused: modify `webantoanmang2.html` or add files under a new `assets/` folder if introducing images/styles.
- Prefer UTF-8 and do not change global line endings or apply broad reformatting to the single HTML file.

5. Integration points & dependencies
- There are no external package manifests (`package.json`, `requirements.txt`, etc.) in this repo. If you add dependencies, include a clear README section and the manifest at repo root.

6. Editing rules for AI agents
- If `.github/copilot-instructions.md` already exists, merge instead of overwrite: preserve any maintainer-supplied notes and append repo-specific items.
- Propose edits as small, single-purpose commits with clear messages (e.g., "fix: update text in webantoanmang2.html to correct typo").
- When adding files, place static assets in `assets/` and reference them with relative paths.

7. Debugging and validation
- Use the browser devtools (console, network) to validate JS and asset loading.
- For content changes, visually verify layout in desktop and mobile widths using the browser responsive tools.

8. When in doubt
- Ask the user/maintainer before introducing new tooling, tests, or CI. This repo's simplicity implies many choices should be confirmed first.

If anything in these instructions is unclear or you want more coverage (CI, tests, or adding build tooling), tell me what to expand.
