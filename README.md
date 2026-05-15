# andrewtrodriguez.com

Personal website and online resume for **Andrew T. Rodriguez, Ph.D.** — Ph.D. scientist in aging biology, scientific reasoning, and frontier AI evaluation.

🌐 **Live site:** [andrewtrodriguez.com](https://andrewtrodriguez.com)

## 🛠️ Tech Stack

- **Static HTML/CSS** — no build step, no JavaScript framework
- **Hosting:** [Vercel](https://vercel.com) on the custom domain `andrewtrodriguez.com`
- **Legacy redirect:** [andrewtrodriguez.github.io](https://andrewtrodriguez.github.io) → `andrewtrodriguez.com` (served from the `gh-pages-redirect` branch via GitHub Pages)
- **Typography:** TT Norms via self-hosted woff2

## 📁 Project Structure

```
.
├── index.html           # Main page
├── 404.html             # Custom 404 (gh-pages-redirect branch)
├── vercel.json          # Vercel config + security headers (CSP, X-Frame-Options)
├── assets/
│   ├── icons/           # Favicons, institution logos
│   └── images/          # Avatar, og-image
├── ai.txt               # AI agent permissions
├── llms.txt             # LLM-readable site summary
├── robots.txt           # Crawler permissions
├── sitemap.xml          # Sitemap with image namespace
└── site.webmanifest     # PWA manifest
```

## 🔍 SEO & Discoverability

- JSON-LD structured data (schema.org `Person`)
- Open Graph and Twitter Card meta tags
- `robots.txt` explicitly allowing major AI crawlers (GPTBot, ClaudeBot, PerplexityBot, etc.)
- `llms.txt` for LLM-readable site summary
- `ai.txt` for AI agent permissions and attribution

## ⚡ Performance

- Zero JavaScript dependencies (only a one-line year updater)
- All assets self-hosted (no third-party requests)
- Total page weight under 400KB including images

## ♿ Accessibility

- Skip-to-content link
- Semantic HTML landmarks (`header`, `main`, `aside`, `footer`, `nav`)
- ARIA labels on navigation regions
- WCAG AA color contrast
- Responsive down to 320px viewport

## 🔒 Security Headers

Configured via `vercel.json`:

- `Content-Security-Policy` (strict, self-only with limited exceptions)
- `X-Frame-Options: DENY`
- `X-Content-Type-Options: nosniff`
- `Referrer-Policy: strict-origin-when-cross-origin`
- `Permissions-Policy` (camera, microphone, geolocation disabled)

## 💻 Local Development

No build step. Open directly or serve locally:

```bash
open index.html
# or
python3 -m http.server 8000
```

## 🚀 Deployment

Push to `main` — Vercel auto-deploys to `andrewtrodriguez.com`.
