# Personal Portfolio Website

A clean, responsive portfolio website built with vanilla HTML, CSS, and JavaScript — no frameworks or build tools required.

**Live site:** [JoshLG18/PortfolioWebsite](https://github.com/JoshLG18/PortfolioWebsite)

---

## Overview

Single-page portfolio showcasing projects and skills across machine learning, quantitative finance, data engineering, and research. Features a filterable project gallery, dark/light theme toggle with system preference detection, and a fully responsive layout.

## Features

- **Filterable project gallery** — filter by category (ML/AI, Quant, Data Engineering, Apps, Research)
- **Dark/light theme** — toggles with a button; persists via `localStorage` and respects `prefers-color-scheme` on first load
- **Responsive design** — mobile-friendly with a 600px breakpoint
- **Zero dependencies** — no npm, no build step, no external JS libraries

## Tech Stack

| Layer | Technology |
|---|---|
| Markup | HTML5 |
| Styling | CSS3 with custom properties (variables) |
| Interactivity | Vanilla JavaScript (ES6+) |
| Fonts | Google Fonts — DM Serif Display, DM Sans |
| Hosting | GitHub Pages / static hosting |

## Project Structure

```
Portfolio Website/
├── index.html          # Entire site — markup, styles, and scripts
├── images/             # Project previews, profile photo, icons
├── attachments/        # CV, dissertation, reports (PDF)
└── README.md
```

## Running Locally

No installation required — just open the file in a browser:

```bash
open index.html
```

Or serve it with a local HTTP server (recommended to avoid browser CORS quirks with local files):

```bash
python -m http.server 8000
# Visit http://localhost:8000
```

## Sections

| Section | Description |
|---|---|
| Hero | Introduction and CV download |
| Skills | Categorised technical skills with proficiency levels |
| Projects | Filterable gallery of 10+ projects |
| Certifications | IBM Data Science Professional Certificate |
| Contact | Email, GitHub, LinkedIn |

## Customisation

All styling is driven by CSS custom properties at the `:root` level in `index.html`. To change the colour scheme, update the variables in the `:root` and `body.dark` blocks:

```css
:root {
  --bg: #f5f3ef;
  --ink: #0e1a2b;
  --gold: #b8922a;
}
```

To add a project, add a new `.project-card` element inside `#projects-grid` in `index.html` and include the relevant tag(s) in `data-tags` (e.g. `data-tags="featured ml-ai"`).

## License

This project is open source. Feel free to use it as a template for your own portfolio — attribution appreciated but not required.
