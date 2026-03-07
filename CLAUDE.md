# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Jekyll static site hosted on GitHub Pages at lr7.digital. Studio landing page for lr7 digital.

## Commands

```bash
# Serve locally (http://localhost:4000)
bundle exec jekyll serve

# Build for production
bundle exec jekyll build
```

## Site Structure

- `_layouts/` - HTML templates
- `_config.yml` - Jekyll configuration (url: https://lr7.digital)
- `index.md` - Homepage (uses splash layout)
- `assets/` - Site-wide images (WebP optimized)
- `robots.txt` - Crawl directives
- `sitemap.xml` - XML sitemap

## Layout Hierarchy

```
splash.html     → Homepage (full-screen hero)
default.html    → Base template
```

## Key Conventions

- Layouts use Liquid templating (`{{ }}`, `{{ | relative_url }}`)
- Meta tags (description, OG, Twitter, canonical) in layouts via frontmatter
- Schema.org JSON-LD in layouts (Organization on homepage)
- Use WebP format for images (optimized from 3.3MB → 176KB for hero image)
- Images should have explicit width/height attributes and lazy loading for below-fold
