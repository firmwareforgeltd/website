# firmwareforge.co.uk

Static website for **FirmwareForge Ltd** — embedded systems & firmware
development consultancy. *Code. Hardware. Impact.*

Deployed to GitHub Pages by `.github/workflows/deploy.yml` on every push to
`main`, served at [firmwareforge.co.uk](https://firmwareforge.co.uk/).

## Layout

- `index.html` — single-page site (hero, services, expertise, about, projects, contact)
- `assets/` — styles, logos, favicons, social card
- `robots.txt`, `sitemap.xml`, `llms.txt` — SEO / AI-crawler support
- Logo sources live in the separate `firmwareforge-logo` folder (print-safe SVGs)

## Local preview

```sh
python3 -m http.server -d . 8000
# open http://localhost:8000
```
