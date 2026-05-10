# andrewtrodriguez.github.io

Personal website for Andrew T. Rodriguez. Live at [andrewtrodriguez.github.io](https://andrewtrodriguez.github.io/).

## Tech Stack

- Static HTML/CSS (no build step, no JS framework)
- [TT Norms](https://www.buckinstitute.org/) typeface via woff2
- Responsive two-column grid layout
- GitHub Pages hosting with automatic deploys on push

## SEO & Discoverability

- JSON-LD structured data (schema.org Person)
- Open Graph and Twitter Card meta tags
- `sitemap.xml` with image namespace
- `robots.txt` explicitly allowing all major AI crawlers
- `llms.txt` for LLM-readable site summary
- `ai.txt` for AI agent permissions

## Performance

- Zero JavaScript dependencies (only a one-line year updater)
- All assets self-hosted (no third-party requests except fonts)
- Total page weight under 400KB including images

## Accessibility

- Skip-to-content link
- Semantic HTML landmarks (`header`, `main`, `aside`, `footer`, `nav`)
- ARIA labels on navigation regions
- Sufficient color contrast (WCAG AA)
- Responsive down to 320px viewport

## Structure

```
/
├── index.html          # Main page
├── assets/
│   ├── images/         # Avatar, og-image
│   └── icons/          # Favicons, institution logos
├── robots.txt          # Crawler permissions
├── sitemap.xml         # Sitemap with image support
├── site.webmanifest    # PWA manifest
├── llms.txt            # LLM-readable summary
├── ai.txt              # AI agent permissions
└── _headers            # Security headers
```

## Local Development

Open `index.html` in a browser. No build step needed.

```bash
open index.html
# or
python3 -m http.server 8000
```
