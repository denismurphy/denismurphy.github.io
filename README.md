# denismurphy.ie

Personal site and portfolio. Built with Hugo, deployed to GitHub Pages.

Live at [denismurphy.ie](https://denismurphy.ie)

---

## Stack

- **[Hugo](https://gohugo.io/)** — static site generator
- **Tailwind CSS v4** — pre-built via CLI, no CDN
- **Self-hosted fonts** — Inter and JetBrains Mono (WOFF2, latin subset)
- **GitHub Actions** — build and deploy on push to `main`

---

## Development

**Prerequisites:** Hugo extended, Node.js (for Tailwind CLI)

```bash
# Install Tailwind CLI (once)
npm install -g @tailwindcss/cli

# Run local dev server
hugo server

# Rebuild Tailwind CSS after adding new utility classes
tailwindcss -i ./static/css/input.css -o ./static/css/tailwind.css --minify
```

---

## Project structure

```
layouts/
  _default/baseof.html   # Base template: canvas, YAML watermark, theme toggle
  index.html             # Homepage
  partials/
    head.html            # Meta, OG tags, fonts, CSS variables, styles
    nav.html             # Navigation bar
static/
  css/tailwind.css       # Pre-built Tailwind output (committed)
  fonts/                 # Self-hosted WOFF2 fonts
  og-image.png           # Open Graph image (1200x630)
content/
  blog/                  # Blog posts (Markdown)
config.toml              # Site config, params
.github/workflows/
  deploy.yml             # Build and deploy to GitHub Pages
```

---

## Deployment

Pushes to `main` trigger the GitHub Actions workflow which builds with `hugo --minify` and deploys to GitHub Pages. The live commit hash is injected at build time via `HUGO_PARAMS_COMMIT` and linked in the footer.

---

## License

MIT
