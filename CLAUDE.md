# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Personal academic website for Mannfred Masahiro Asada Boehm (ecologist/ornithologist), hosted via GitHub Pages at mannfred.github.io. The site is static hand-maintained HTML — there is no build step, no framework, and no package manager.

## Structure

- `docs/index.html` — the entire website (single page, all content lives here)
- `docs/style.css` — shared stylesheet (Courier New font, powder blue palette, container-based layout)
- `docs/media/` — images and PDFs referenced by the page

GitHub Pages is configured to serve from the `docs/` folder on the `main` branch.

## Development workflow

Edit `docs/index.html` (and `docs/style.css` as needed), then commit and push. GitHub Pages deploys automatically on push to `main`. No build commands are required.

## Key conventions

- **Bilingual content**: The page mixes English and Japanese. Japanese text uses `<ruby>` tags with `<rt>` for furigana (pronunciation guides).
- **Layout**: Absolute-positioned overlay on a full-bleed background image; content constrained to ~600–1000px max-width.
- **Publications**: Listed as inline links pointing to PDF files in `docs/media/` or external DOIs.
- The `.Rproj` file is vestigial — the site is no longer generated via R.
