# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static archive of "Needles + Leaves," a succulent blog that was originally built on Squarespace. The site has been exported as static HTML files and cleaned up to remove unnecessary Squarespace functionality for use as a static archive hosted on GitHub Pages. The domain `needlesandleaves.net` is configured via the CNAME file.

### Archive Status
This is a **cleaned static archive** - all dynamic Squarespace features have been intentionally removed to create a lightweight, functional static website that preserves the original content and styling without server dependencies.

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

### Asset Management - CLEANED
- **CSS files**: Preserved essential styling and layout files (175 remaining)
- **JavaScript files**: Reduced to essential layout and font loading only (106 remaining, down from 400+)
- **Images**: All original content images preserved (694 files)
- **Removed**: All commerce, analytics, social media, comments, and dynamic functionality

### Files Removed During Cleanup (400+ files)
The following unnecessary Squarespace features were removed:
- Analytics and tracking scripts (`analytics.js`)
- E-commerce functionality (`commerce-*.js`, `commerce-*.css`)
- ReCAPTCHA and security features (`recaptcha__en.js`)
- Enterprise features (`enterprise.js`)
- Comments system (`comments-*.js`, `comments-*.css`)
- Social media integration (`social-buttons-*`, `simple-liking-*`)
- Performance monitoring (`performance-*.js`)
- Dynamic JavaScript libraries (`common-*.js`, `extract-css-*`)
- Duplicate and temporary files

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
- **CSS files**: Essential styling preserved, safe to modify for layout tweaks
- **JavaScript files**: Only essential layout and TypeKit font loading remain
- Local assets should be placed in appropriate `_files/` directories
- **Do not add back**: Commerce, analytics, social, or dynamic Squarespace features

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

## Archive Cleanup History

### What Was Cleaned (2024)
This archive underwent extensive cleanup to remove unnecessary Squarespace functionality:

**Total files removed**: 400+ files
**HTML files cleaned**: 47 files (removed script references to deleted assets)
**File count**: Reduced from 3,000+ to 2,544 files
**Focus**: Preserved all content, styling, and images while removing server-dependent features

### Remaining File Types
- **49 HTML files**: All blog posts and pages preserved
- **175 CSS files**: Essential styling for layout and design
- **106 JavaScript files**: Only layout essentials and TypeKit font loading
- **694 Image files**: All original photography and graphics
- **2,544 total files**: Clean, functional static archive

## Important Notes

- This is a **cleaned static archive** from Squarespace, optimized for static hosting
- No modern build tools, frameworks, or package managers are used
- The site structure reflects Squarespace's export format
- **All dynamic functionality has been intentionally removed** for static compatibility
- Content is primarily focused on succulents, gardening, and DIY crafts
- Archive preserves the original design and all content from the active blog years (2013-2020)

## Maintenance Guidelines

### What NOT to Add Back
- Analytics or tracking scripts
- E-commerce functionality 
- Social media integration
- Comments systems
- Any server-dependent features

### Safe to Modify
- CSS styling and layout
- Image content and optimization
- HTML content within existing structure
- Static navigation and links