# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Personal brand/portfolio landing page for cmondor.com. Plain HTML/CSS — no build step, no frameworks, no dependencies. Hosted on Netlify via drag-and-drop or git integration.

## Local Development

```
npm run dev
```

Starts `netlify dev` at `http://localhost:8888`. Mirrors the production environment including headers defined in `netlify.toml`. Requires Netlify CLI installed (`npm install -g netlify-cli`).

## Deployment

- Deploy by pushing to the connected git branch, or drag the project folder into the Netlify dashboard.
- No build command. Publish directory is the repo root.
- `netlify.toml` sets security headers and cache-control rules.

## Structure

- `index.html` — single-page layout with sections: hero, about, work, contact
- `styles.css` — all styles; uses CSS custom properties defined in `:root` for theming
- `netlify.toml` — Netlify headers and cache configuration

## Conventions

- All theming (colors, spacing, typography) is controlled via CSS variables in `:root` at the top of `styles.css`.
- No JavaScript frameworks. Inline `<script>` tags are acceptable for minimal interactivity.
- Keep the page as a single `index.html`. Add new HTML files only for distinct pages (e.g. `404.html`).
- Every HTML page must include the Google tag snippet (G-3HNB8D27RV) in the `<head>` before other resource tags.
