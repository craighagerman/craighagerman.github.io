# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

@AGENTS.md

`AGENTS.md` (imported above) is the **authoritative, tool-neutral entry point** — read it first. It covers the repo's layout, the "route your change" table, the silent-failure gotchas, and the local command set. Keep shared guidance in `AGENTS.md` (Codex reads it directly) and put only Claude-specific notes below, so Claude and Codex stay in sync.

## Claude-specific notes

- This is a personal, single-author site with no test suite. "Verify your change" means: `bundle exec jekyll build --strict_front_matter` (matches CI) plus a visual check with `bundle exec jekyll serve`. Prefer small, direct edits over scaffolding.
- Don't hand-edit generated files — regenerate them: `_data/cv.json` (via `bash scripts/update_cv_json.sh`), `assets/js/main.min.js` (via `npm run build:js`), and `talkmap_out.ipynb` / `talkmap/` (auto-generated in CI).
- When you edit `_pages/cv.md` or any `assets/js/` source, include the regenerated output in the same change.
