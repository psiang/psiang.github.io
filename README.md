# Sixiang Peng's research homepage

Public site: https://psiang.github.io/

Plain HTML and CSS, served by GitHub Pages from `master` at the repository root. No build step or dependencies are required. `.nojekyll` keeps the published files unchanged.

- `index.html`: biography, publications, manuscripts, and contact details.
- `assets/home.css`: responsive homepage styles.
- `blog/`: migrated snapshot of the 2020 Hexo / Butterfly blog.
- Existing article, tag, archive and category HTML paths redirect to `/blog/`, preserving query strings and fragments. Original image and script paths remain available for old external links.

## Blog preservation

The complete pre-migration published site and its existing Git history remain at branch `backup/blog-before-homepage-20260930`, commit `eaabf23130081c95ba3be936f6fa8b546726ff44`. Do not delete or force-push this branch.

The original repository contains generated static output only. Hexo Markdown sources, theme source, and build configuration were not present and must be recovered separately if future Hexo regeneration is desired. Do not run an old Hexo deployment over this repository root; generate future blog output under `blog/`.

The archived article text and bundled images are preserved. Broken pre-existing menu entries (About, Links, Movies, Music) were removed; the missing avatar is replaced by a monogram; a feed and research-homepage link were added. Some externally hosted 2020 assets or third-party services may no longer be available.

## Editing

Edit `index.html` and `assets/home.css`, then commit to `master`. Preview with `python -m http.server 8000`.

The research profile presents program analysis and formal reasoning as complementary approaches to reliable foundation-model agents. SPONGE covers efficient interactive analysis; ReCoNav covers task formalization and agent decision checking. Speculative future applications are not listed as completed work.

SPONGE metadata was verified against its final source and the HKUST research portal. Its assigned ACM DOI was not resolving at launch, so the publication link uses the HKUST record. ReCoNav is listed as a manuscript under review with its submitted title and a short description; add a full author list and a preprint link once verified public resources are available.

## Restore the old site without rewriting history

Create a fresh branch from the latest `master`. Restore the tracked tree from the backup commit (including removing files absent from that commit), review it, then commit and merge that restoration. Do not reset or force-push `master`.
