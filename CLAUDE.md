# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with
code in this repository.

## Project Overview

This is a Hugo static site for ElecPower/Wetown Electric Group (Stock Code: 688226), a global manufacturer of high-voltage busbar systems (IPB), energy storage systems, and power distribution equipment. The site is deployed to GitHub Pages via GitHub Actions and uses the Hugoplate theme.

## Build & Deploy Commands

### Local Development

```bash
# Install Hugo (if not already installed)
# macOS: brew install hugo
# Windows: scoop install hugo or choco install hugo

# Start local development server
hugo server

# Build the site for production
hugo --minify
```

### Theme Setup

The Hugoplate theme requires npm dependencies:

```bash
# Navigate to theme directory (must be initialized as git submodule first)
cd themes/hugoplate

# Install npm dependencies
npm install

# Return to project root
cd ../..
```

### Git Operations

```bash
# Initialize hugoplate theme as git submodule (first time setup)
git submodule add https://github.com/gethugothemes/hugoplate.git themes/hugoplate

# Update theme submodule
git submodule update --remote --merge

# Stage all changes (including submodule updates)
git add .

# Commit with conventional commit format
git commit -m "feat: add new blog post about IPB specifications"

# Push to main branch (triggers GitHub Actions deployment)
git push origin main
```

### GitHub Actions Deployment

Deployment is automated via `.github/workflows/hugo.yml`:

- Trigger: Push to `main` branch or manual workflow dispatch
- Build environment: Ubuntu Latest
- Hugo version: latest (extended)
- Node.js version: 20
- Deployment target: GitHub Pages (gh-pages branch)

**Workflow Steps:**
1. Checkout with recursive submodules
2. Setup Hugo (extended)
3. Setup Node.js v20
4. Install theme dependencies (`cd themes/hugoplate && npm install`)
5. Build with minification (`hugo --minify`)
6. Deploy to GitHub Pages

## Project Architecture

### Directory Structure

```
elecpower-blog-new/
├── .github/
│   └── workflows/
│       └── hugo.yml           # GitHub Actions CI/CD pipeline
├── content/
│   └── english/
│       ├── _index.md           # Homepage (Hugoplate frontmatter)
│       ├── blog/               # Blog posts
│       │   └── ipb-technical-overview.md
│       └── contact/
│       │   └── _index.md       # Contact page
├── themes/
│   └── hugoplate/              # Git submodule: Hugoplate theme
├── public/                     # Hugo build output (gitignored)
├── hugo.toml                   # Hugo configuration file
└── CLAUDE.md                  # This file
```

### Content Architecture

**Hugoplate Frontmatter Pattern:**

```yaml
---
# Required for homepage
title: "Page Title"
meta_title: "SEO Title"
description: "Page description for SEO"

# Homepage specific sections
banner:
  title: "Banner Title"
  content: "Banner content text"
  button:
    enable: true
    label: "Button Label"
    link: "/target-url"

features:
  - title: "Feature Title"
    image: "/images/path.png"
    content: "Feature description"
    bulletpoints:
      - "**Bold Point:** Description"
    button:
      enable: true
      label: "Button Text"
      link: "/target-page"
---
```

**Blog Post Frontmatter Pattern:**

```yaml
---
title: "Post Title"
description: "Post description"
date: 2025-03-11
draft: false
tags: ["IPB", "busbar", "power distribution"]
categories: ["Technical Guide"]
og_image: ""
---
```

### Hugo Configuration Key Points (hugo.toml)

- **Base URL**: `https://www.elecpower.cn/`
- **Theme**: hugoplate
- **Time Zone**: America/New_York
- **Default Language**: English
- **Content Location**: `content/english/`
- **Imaging**: Quality 80, Lanczos resampling
- **Custom Parameters** (lines 168-177):
  - description: SEO description
  - keywords: Array of SEO keywords
  - author: 'ElecPower Team'
  - contact: 'andyzhu716@gmail.com'

## Content Guidelines

### Technical Specifications

When writing technical content about electrical equipment:

1. **Use Precise Terminology**:
   - Isolated Phase Bus → IPB
   - NSPB/SPB → Medium-Voltage Enclosed Bus
   - CRB → Cast Resin Busway
   - PJTM → Insulated Copper Tube Busbar

2. **Technical Accuracy**: Reference IEEE standards (e.g., IEEE C37.23 for IPB)

3. **Specification Format**:
   - Use markdown tables for parameters
   - Include typical ranges and standards
   - Note safety ratings (IP54, IP65, IP68)

### SEO Best Practices

- Maintain keywords consistency with hugo.toml `keywords` array
- Use descriptive meta_title and description
- Include og_image for blog posts
- Keep descriptions under 160 characters for optimal search display

### Brand Guidelines

- **Company Name**: Wetown Electric Group / ElecPower
- **Stock Code**: 688226 (include when relevant)
- **Contact Email**: andyzhu716@gmail.com
- **Core Products**: IPB, NSPB, SPB, CRB, PJTM, Power Transformers, ESS, PV Materials

## Common Development Tasks

### Adding a New Blog Post

```bash
# Create new blog post
cat > content/english/blog/new-post.md << 'EOF'
---
title: "New Technical Guide"
description: "Brief description"
date: 2025-03-18
draft: false
tags: ["tag1", "tag2"]
categories: ["Technical Guide"]
og_image: ""
---

# Content here in markdown
EOF

# Preview locally
hugo server

# Commit and deploy
git add content/english/blog/new-post.md
git commit -m "feat: add blog post about [topic]"
git push origin main
```

### Updating Homepage Content

Edit `content/english/_index.md` sections (banner, features). The Hugoplate theme uses specific frontmatter keys:
- `banner`: Hero section
- `features`: Feature cards with images, bullet points, and optional buttons

### Updating Navigation

Navigation is typically managed through Hugoplate theme configuration or Hugo's built-in menu system. Check theme documentation for specific methods.

## Troubleshooting

### Build Failures

1. **Missing Theme Submodule**:
   ```bash
   git submodule update --init --recursive
   ```

2. **Theme Dependencies Missing**:
   ```bash
   cd themes/hugoplate && npm install
   ```

3. **Image Paths**: Use relative paths from `/images/` root, verify image exists before building

### Deployment Issues

- Check `.github/workflows/hugo.yml` is committed to main branch
- Verify GitHub Pages is enabled in repository settings
- Check deployment logs in Actions tab for specific errors

## Git Branch Strategy

- **main**: Production branch, pushes trigger deployment to GitHub Pages
- **gh-pages**: Automatically managed by GitHub Actions (do not work directly on this branch)
- **feature branches**: Create for new content/features, merge to main when ready

## External Resources

- **Hugoplate Theme**: https://github.com/gethugothemes/hugoplate
- **Hugo Documentation**: https://gohugo.io/
- **GitHub Pages**: https://docs.github.com/en/pages
