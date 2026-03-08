# AGENTS.md

Agent instructions for working with this repository (Claude Code, Gemini CLI, etc.).

## Project Overview

Static site hosted on GitHub Pages at lr7.digital. Studio landing page for lr7 digital.

> Note: The site is plain HTML (`index.html`) — no Jekyll build step required for the current site. Jekyll config is retained for historical reference.

## Commands

```bash
# Serve locally
python3 -m http.server 4100

# Jekyll (legacy)
bundle exec jekyll serve   # http://localhost:4000
bundle exec jekyll build
```

## Site Structure

- `index.html` - Homepage
- `assets/` - Site-wide images (WebP optimized)
- `robots.txt` - Crawl directives
- `sitemap.xml` - XML sitemap
- `_config.yml` - Jekyll configuration (url: https://lr7.digital)

## Key Conventions

- Use WebP format for images (optimized from 3.3MB → 176KB for hero image)
- Images should have explicit width/height attributes and lazy loading for below-fold
- Meta tags (description, OG, Twitter, canonical) defined inline in `index.html`
- Schema.org JSON-LD included in `index.html` (Organization type)
- Prepend `bundle exec` to `jekyll` commands to avoid gem version conflicts
