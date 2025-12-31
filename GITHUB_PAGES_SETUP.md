# GitHub Pages Setup Guide

Your About-Me repository is now configured as a Jekyll-based GitHub Pages site!

## Steps to Enable GitHub Pages

1. **Rename your repository** (if you haven't already):
   - Go to your repository settings on GitHub
   - Rename the repository to: `aparnarvm.github.io`
   - Your site will automatically be published at: `https://aparnarvm.github.io`

2. **Enable GitHub Pages** (usually automatic for a repo named `username.github.io`):
   - Go to repository Settings → Pages
   - Source should be set to "Deploy from a branch"
   - Branch: select `main` (or `master`) and root folder `/`
   - Click Save

3. **Wait for the build**:
   - GitHub will automatically detect the Jekyll configuration
   - You'll see a notification when your site is live
   - Check the "Actions" tab to monitor the build process

## What's Included

- **_config.yml**: Jekyll configuration with your profile information
- **index.md**: Your homepage with all your content formatted nicely
- **Gemfile**: Dependencies for Jekyll and GitHub Pages

## Customization

### Change the Theme
The site uses the `minima` theme by default (light, clean design). To change it, edit `_config.yml`:
```yaml
theme: jekyll-theme-minimal  # Try: minimal, hacker, midnight, etc.
```

### Add More Pages
Create new `.md` files in the root directory:
```
about.md
projects.md
blog.md
```

Each file should start with front matter:
```yaml
---
layout: page
title: About
---

Your content here...
```

### Local Testing
To preview changes locally:
```bash
bundle install
bundle exec jekyll serve
```
Then visit `http://localhost:4000`

## Documentation
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Jekyll Documentation](https://jekyllrb.com/)
- [Minima Theme Documentation](https://github.com/jekyll/minima)
