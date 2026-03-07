- Prepend `bundle exec` to `jekyll` commands to avoid gem version conflicts.

# GEMINI.md - Project Context for lr7 digital

## Project Overview
This repository contains the source code for the `lr7 digital` studio website, hosted at `https://lr7-digital.github.io`. The site is a static website built using **Jekyll** and serves as the studio landing page.

## Core Technologies
- **Jekyll**: Static site generator used to build the project.
- **Liquid**: Templating engine for Jekyll layouts and pages.
- **GitHub Pages**: The hosting platform for the live site.
- **Ruby**: Required for running Jekyll locally via Bundler.

## Key Directories and Files
- `_config.yml`: Global configuration for the Jekyll site, including site metadata and build settings.
- `_layouts/`: Contains HTML templates that define the site's structure:
    - `default.html`: The base layout with navigation and global styles.
    - `splash.html`: Full-screen hero layout for the homepage.
- `index.md`: The root landing page for the `lr7 digital` studio.
- `Gemfile`: Lists Ruby dependencies (primarily `github-pages` gem).

## Building and Running Locally

### Prerequisites
- Ruby and Bundler installed.

### Setup
1.  Install dependencies:
    ```bash
    bundle install
    ```

### Local Development
1.  Start the Jekyll server:
    ```bash
    bundle exec jekyll serve
    ```
2.  Open your browser to `http://localhost:4000`.

## Development Conventions
- **Static Content**: Most content is written in Markdown (`.md`) files with Front Matter for layout and metadata.
- **Relative URLs**: Use the `{{ '/path/' | relative_url }}` filter for internal links to ensure they work correctly across different environments (local vs. production).
- **Styling**: Global styles are in layout files within `<style>` tags.
