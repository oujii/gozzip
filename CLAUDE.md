# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A modern Jekyll blog named "Gozzip" designed for GitHub Pages hosting. The blog covers trending topics, culture, and discussions from around the web with a clean, responsive design.

## Architecture

- **Framework**: Jekyll static site generator
- **Platform**: GitHub Pages compatible
- **Styling**: Custom CSS with Inter font family
- **Structure**: Standard Jekyll directory layout with custom pages

## Key Directories

- `_posts/` - Blog posts (YYYY-MM-DD-title.md format)
- `_pages/` - Static pages (about, archive, categories)
- `_layouts/` - Page templates (default, post, page)
- `_includes/` - Reusable HTML components (header, footer)
- `assets/` - CSS, JS, and images

## Development Commands

```bash
# Install dependencies
bundle install

# Start local development server
bundle exec jekyll serve

# Build for production
bundle exec jekyll build

# Clean build artifacts
bundle exec jekyll clean
```

## Configuration

- **Site config**: `_config.yml` - contains site metadata, navigation, and Jekyll settings
- **Dependencies**: `Gemfile` - locked to GitHub Pages compatible versions
- **Styling**: `assets/css/main.css` - primary stylesheet with CSS variables

## Content Creation

### New Blog Post
1. Create file in `_posts/` with format: `YYYY-MM-DD-title.md`
2. Add front matter:
   ```yaml
   ---
   layout: post
   title: "Post Title"
   date: YYYY-MM-DD
   categories: [category1, category2]
   tags: [tag1, tag2]
   ---
   ```

### New Static Page
1. Create file in `_pages/` directory
2. Add to navigation in `_config.yml` under `navigation:` section

## Deployment

- **GitHub Pages**: Automatically deploys from main branch
- **Custom domain**: Add `CNAME` file to root directory
- **URL**: `https://username.github.io/repository-name`