# AGENTS.md - Pragmore Website

## Project Overview

This is the static website for **Pragmore** - a software development company focused on AI-augmented development with senior oversight. The site is hosted on GitHub Pages.

- **URL**: https://pragmore.com
- **Repository**: pragmore/pragmore.github.io
- **Type**: Static HTML website

## Technology Stack

- **HTML5** - Semantic markup
- **CSS3** - Custom styles in `template.css` and `theme.css`
- **Bootstrap 4.1.1** - CSS framework via CDN
- **Devicon** - Technology icons via CDN (https://devicon.dev/)
- **Ionicons 3.0** - UI icons via CDN

## File Structure

```
/
├── index.html          # Main page (single-page site)
├── theme.css           # Bootstrap theme customizations
├── template.css        # Additional custom styles
├── logo.png            # Company logo
├── favicon.ico         # Favicon files
├── CNAME               # Custom domain config (pragmore.com)
└── site.webmanifest    # PWA manifest
```

## Sections

1. **Header/Hero** (`#contact-us`) - Main tagline and CTA
2. **Navigation** (`#navbar1`) - Fixed top navbar with anchor links
3. **What We Do** (`#what-we-do`) - Three service cards:
   - Solve problems
   - Senior oversight  
   - Staff augmentation
4. **Technologies** (`#technologies`) - Tech stack showcase organized by:
   - Backend (Python, Node.js, PHP, Laravel, Rails, Symfony, GraphQL)
   - Frontend (React, Next.js, Vue.js, Angular, TypeScript, React Native)
   - Data & Cloud Platform (PostgreSQL, MySQL, MongoDB, Redis, AWS, Google Cloud)
5. **Who We Are** (`#who-we-are`) - Company description
6. **Footer** - Social links and contact email

## Guidelines for Changes

### Styling
- Use existing Bootstrap 4 classes when possible
- Custom styles go in `template.css`
- Primary color: Bootstrap's `bg-primary` (blue)
- Tech logos: Use Devicon CDN URLs with consistent format:
  ```
  https://cdn.jsdelivr.net/gh/devicons/devicon/icons/{tech}/{tech}-original.svg
  ```

### Adding Technologies
When adding new tech items:
1. Use `col-4 col-md-2 mb-4` for consistent grid layout
2. Structure:
   ```html
   <div class="col-4 col-md-2 mb-4">
       <div class="tech-item text-center">
           <img src="..." alt="Name" class="tech-logo">
           <p class="small mt-2 mb-0">Name</p>
       </div>
   </div>
   ```

### Images
- Tech logos: 50x50px (controlled by CSS `.tech-logo`)
- Logo: 100x100px

## Deployment

The site auto-deploys via GitHub Pages when pushing to the `master` branch.

## Contact

- Email: hi@pragmore.com
- Social: LinkedIn, Twitter/X, GitHub (links in footer)
