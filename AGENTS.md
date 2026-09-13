# Agent Guidelines for Academic Pages (craighagerman.github.io)

**This file is the authoritative, tool-neutral entry point for coding agents (Claude Code, Codex, etc.) working in this repo. Read it before making changes.** Claude-specific notes live in `CLAUDE.md`, which imports this file — so keep shared facts here, not there.

This is a personal academic / portfolio website built from the [academicpages](https://github.com/academicpages/academicpages.github.io) Jekyll template (itself derived from Minimal Mistakes) and deployed with GitHub Pages. It was created from that template for personal use — there is **no need** to open a pull request back to the upstream `academicpages.github.io` repository.

**The theme is vendored directly in this repo.** There is no theme gem and no `remote_theme`: `_layouts/`, `_includes/`, `_sass/`, and `assets/` are all editable here, and editing them is the intended way to change the site's look and behavior. (If you've seen the al-folio template, this is the opposite of its "runtime lives in gems" model — nothing here is off-limits for that reason.)

## Route your change

| Your change | Goes in |
| --- | --- |
| Page content (About, CV page, standalone pages) | `_pages/` (e.g. `about.md`, `cv.md`) |
| Blog posts / drafts | `_posts/` / `_drafts/` |
| Publication, talk, teaching, or portfolio entries | the matching collection — `_publications/`, `_talks/`, `_teaching/`, `_portfolio/` (one Markdown file per item) |
| Nav menu, author/profile info, UI strings | `_data/navigation.yml`, `_data/authors.yml`, `_data/ui-text.yml` |
| Structured CV data | edit `_pages/cv.md`, then regenerate `_data/cv.json` (see gotchas) — don't hand-edit `cv.json` |
| Site config, plugins, collections, defaults | `_config.yml` (and `_config_docker.yml` for local Docker) |
| Layout / page HTML structure | `_layouts/`, `_includes/` |
| Styles | `_sass/` (compiled through `assets/css/main.scss`) |
| Client-side JS | `assets/js/_main.js`, `assets/js/plugins/*`, `assets/js/theme.js` → then rebuild `main.min.js` (see gotchas) |

## Gotchas that produce no obvious error

1. **`_data/cv.json` is generated.** It's produced from `_pages/cv.md` by `scripts/update_cv_json.sh` (which calls `scripts/cv_markdown_to_json.py`). Edit the Markdown and regenerate — hand edits to `cv.json` get overwritten on the next run.
2. **Publications and talks can be bulk-generated.** `markdown_generator/publications.py` and `markdown_generator/talks.py` turn the `*.tsv`/`*.csv` files there into per-item Markdown in `_publications/` and `_talks/`. Editing individual collection files by hand is fine, but re-running a generator regenerates the whole set.
3. **The talk map auto-commits.** Pushing changes under `_talks/**` (or `talkmap.ipynb`) triggers `.github/workflows/scrape_talks.yml`, which geocodes talk locations and pushes a **bot commit** updating `talkmap_out.ipynb` and `talkmap/`. Expect a follow-up commit after such a push.
4. **JS is served pre-minified.** The site loads `assets/js/main.min.js`. After editing `assets/js/_main.js`, `theme.js`, or a plugin, run `npm run build:js` to rebuild it — source edits alone won't show up.
5. **Plugins are limited to the GitHub Pages allowlist.** The `Gemfile` uses the `github-pages` gem, so only GitHub-Pages-supported plugins run on the deployed site. Adding an arbitrary Jekyll plugin to `_config.yml` silently does nothing in production.
6. **CI builds with `--strict_front_matter`.** `.github/workflows/jekyll-build.yml` runs `bundle exec jekyll build --strict_front_matter` (Ruby 3.2, `JEKYLL_ENV=production`). Malformed or missing front matter fails the build even when local `jekyll serve` tolerates it.

## Local commands

```bash
bundle install                                  # install Ruby gems
bundle exec jekyll serve                        # dev server → http://localhost:4000
bundle exec jekyll build --strict_front_matter  # match the CI build

npm install && npm run build:js                 # rebuild assets/js/main.min.js after JS edits
npm run watch:js                                # rebuild on JS change

bash scripts/update_cv_json.sh                  # regenerate _data/cv.json from _pages/cv.md
python3 publications.py                          # from markdown_generator/: TSV/CSV → _publications/*.md (talks.py for _talks)

docker compose up                                # serve via Docker (merges _config.yml + _config_docker.yml) → :4000
```

## Before you commit

- This is a personal site — commit to this repo; do not PR upstream.
- If you touched `_pages/cv.md`, regenerate `_data/cv.json` in the same change.
- If you touched anything under `assets/js/`, rebuild and commit `assets/js/main.min.js`.
- Keep front matter valid so the strict CI build passes.
