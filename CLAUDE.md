# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static website for "Needles + Leaves," a succulent blog and online shop hosted on GitHub Pages. The site was originally built on Squarespace and has been exported as static HTML files. The domain `needlesandleaves.net` is configured via the CNAME file.

## Site Architecture

### Static HTML Structure
- **Main Pages**: `index.html`, `about.html`, `blog.html`, `diyandtutorials.html`, `lifestyle-1.html`, `succulent-help.html`, `succulents.html`
- **Blog Structure**: Organized by year and date in `/blog/YYYY/MM/DD/` format with individual HTML files for each post
- **Assets**: Each page has an associated `_files/` directory containing CSS, JS, and image assets

### Key Directories
- `/blog/` - Blog posts organized chronologically from 2013-2020
- `/lifestyle/` - Lifestyle content with similar date-based structure
- Various `*_files/` directories - Contains page-specific assets (CSS, JS, images)

### Content Categories
- **Blog Posts**: Succulent care guides, propagation tutorials, garden tours
- **DIY Tutorials**: Step-by-step craft projects featuring succulents
- **Succulent Help**: Plant care advice and troubleshooting
- **Lifestyle**: Personal content and photography

## Technical Details

### Hosting & Deployment
- **Platform**: GitHub Pages
- **Domain**: needlesandleaves.net (configured via CNAME)
- **Deployment**: Automatic via GitHub Pages on push to main branch

### Asset Management
- CSS files are minified Squarespace assets
- JavaScript includes Squarespace platform code, analytics, and social features
- Images are referenced from Squarespace CDN and local assets

### No Build Process
This is a static site with no build system, package.json, or development dependencies. All files are served directly as-is.

## Development Guidelines

### File Management
- HTML files are exported from Squarespace with specific formatting
- Asset files follow Squarespace naming conventions
- When adding new content, maintain the existing directory structure

### Content Updates
- Blog posts follow the `/blog/YYYY/MM/DD/post-title.html` pattern
- Each post should have a corresponding `_files/` directory for assets
- Maintain consistent metadata in HTML head sections

### Asset Handling
- Images should be optimized for web use
- CSS and JS files are primarily Squarespace-generated
- Local assets should be placed in appropriate `_files/` directories

## Common Tasks

### Adding New Blog Posts
1. Create directory structure: `/blog/YYYY/MM/DD/`
2. Create HTML file with post content
3. Create corresponding `_files/` directory for assets
4. Update navigation/index pages as needed

### Updating Existing Content
1. Locate the specific HTML file
2. Edit content within the Squarespace-generated structure
3. Update associated assets in the `_files/` directory

### Domain Management
- Domain configuration is handled via the CNAME file
- DNS settings are managed externally

## Important Notes

- This is a static export from Squarespace, not a typical web development project
- No modern build tools, frameworks, or package managers are used
- The site structure reflects Squarespace's export format
- All dynamic functionality is handled via embedded Squarespace JavaScript
- Content is primarily focused on succulents, gardening, and DIY crafts