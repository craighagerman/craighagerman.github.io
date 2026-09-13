# How to remove or hide pages


**To hide it from the nav:** comment out or delete its entry in `_data/navigation.yml`.

**To remove the URL as well:** stop Jekyll from generating that page. The usual way is to delete (or move) the file in `_pages/` that sets the permalink, such as:

- `_pages/portfolio.html` → `/portfolio/`
- `_pages/talks.html` → `/talks/`
- `_pages/teaching.html` → `/teaching/`

If you want to keep the file around, you can instead set `published: false` in its front matter, or add the file to `exclude:` in `_config.yml`.

One extra catch: listing pages like Talks, Teaching, and Portfolio also have collection items (`_talks/`, `_teaching/`, `_portfolio/`). Those still get their own URLs while `output: true` is set for that collection in `_config.yml`. Removing the listing page does not remove `/talks/some-talk/` and similar paths. To drop those too, set that collection’s `output` to `false`, or remove/unpublish the items.

The HTML sitemap at `/sitemap/` lists every generated page automatically, so once a page is unpublished it drops out of there as well.