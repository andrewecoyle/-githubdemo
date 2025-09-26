# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A personal portfolio website built with pure HTML and CSS. Each page is self-contained with embedded styles and can be viewed directly in any browser without a build process.

## Architecture

The site follows a simple multi-page architecture:

- **index.html** - Homepage with navigation to all other pages
- **about.html** - Personal about page
- **linkedin.html** - LinkedIn profile snapshot
- **movies.html** - Favorite movies list
- **music-producers.html** - Favorite music producers ranking
- **philosophers.html** - Philosophy-related content
- **favorite-books.html** - Favorite books list

## Styling Patterns

All pages follow consistent styling patterns:
- Shared CSS embedded in each HTML file (no external stylesheets)
- Current color scheme: `#FF8F8F` background (coral/salmon), `#fff` containers, `#0066cc` links
- Flexbox centering with `.container` class for main content
- `.nav-links` class for navigation with consistent styling and vertical layout
- Full viewport coverage with `height: 100vh` on body
- Consistent typography using Arial sans-serif font family

## Development Workflow

Since this is a static site with no build tools:
- Edit HTML files directly
- No package.json or npm commands available
- Test by opening HTML files in browser or using a simple HTTP server
- Git workflow: create feature branches, commit changes, push to remote

## Content Patterns

When adding new pages:
1. Follow the existing HTML structure and styling patterns
2. Include navigation back to home page
3. Add navigation link from index.html to new page
4. Use consistent container and styling classes
5. Maintain the same responsive design approach

## Git Branch Strategy

The repository uses feature branches for new content:
- `main` - stable branch
- Feature branches for individual pages (e.g., `music-producers-page`)
- Clean commit messages following existing patterns as necessary. 