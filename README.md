# GIS Portfolio — Jekyll + GitHub Pages

An editorial, bold portfolio site for GIS professionals. Built with Jekyll, deployable to GitHub Pages in minutes.

---

## 🚀 Quick Start

### 1. Clone & Install

```bash
git clone https://github.com/YOURUSERNAME/YOURUSERNAME.github.io
cd YOURUSERNAME.github.io
bundle install
```

### 2. Run Locally

```bash
bundle exec jekyll serve
# Open http://localhost:4000
```

### 3. Deploy to GitHub Pages

Push to a repo named `YOURUSERNAME.github.io` — GitHub Pages will build it automatically.

Or for a project page, push to any repo and set **Settings → Pages → Source → main branch**.

---

## ✏️ Customise

### Personal Info (`_config.yml`)

```yaml
title: "GIS Portfolio"
author: "Your Name"
email: "your@email.com"
github: "yourgithub"
linkedin: "yourlinkedin"
```

### Add a Project

Create a new file in `_projects/`:

```markdown
---
title: "My Project Title"
summary: "One-sentence description shown on the homepage grid."
category: Web Mapping          # Web Mapping | Remote Sensing | Spatial Analysis | Cartography
thumb_class: webmap            # webmap | remote | analysis | carto
tools: [Mapbox GL JS, Python]
year: 2024
role: GIS Analyst
dataset: OpenStreetMap
order: 5                       # Controls sort order in grid
github_url: https://github.com/...    # optional
live_url: https://...                  # optional
---

Write your project description here in Markdown.
Use ## headings for sections like Overview, Methodology, Results.
```

### Thumbnail Colour Themes

| `thumb_class` | Colour scheme |
|---|---|
| `webmap` | Dark blue gradient |
| `remote` | Forest green |
| `analysis` | Purple/magenta |
| `carto` | Warm amber/brown |

Add your own real screenshots by replacing the `.thumb--*` CSS backgrounds with:
```css
.thumb--myproject { background-image: url('/assets/images/myproject.jpg'); background-size: cover; }
```

---

## 📁 Structure

```
├── _config.yml          # Site settings
├── _layouts/
│   ├── default.html     # Base layout (header + footer)
│   └── project.html     # Individual project page
├── _includes/
│   ├── nav.html
│   └── footer.html
├── _projects/           # One .md file per project
├── assets/
│   ├── css/main.css
│   ├── js/main.js
│   └── images/          # Add your screenshots here
└── index.html           # Homepage
```

---

## 🎨 Design Customisation

All design tokens are CSS variables at the top of `assets/css/main.css`:

```css
:root {
  --ink:     #0d0d0d;    /* Primary dark */
  --paper:   #f5f0e8;    /* Background */
  --accent:  #c8401a;    /* Red accent (CTAs, highlights) */
  --accent-2:#2a4a6b;    /* Blue accent */
  --accent-3:#4a7c59;    /* Green accent */
}
```
