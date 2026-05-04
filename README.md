# Andrew T. Rodriguez — GitHub Pages Portfolio

This repository powers the public site at:

- **https://andrewtrodriguez.github.io/**

## What is included

- `index.html` — single-page portfolio landing page.
- `robots.txt` — crawl policy for search engines.
- `sitemap.xml` — sitemap for indexing.
- `.github/workflows/deploy-pages.yml` — CI + deployment workflow for GitHub Pages.

## GitHub Pages setup (required once)

In the repository on GitHub:

1. Open **Settings → Pages**.
2. Set **Build and deployment → Source** to **GitHub Actions**.

## Deployment behavior

The workflow does two things:

1. **Verify** on pushes, pull requests, and manual runs:
   - checks `index.html`, `robots.txt`, and `sitemap.xml` exist.
2. **Deploy** only when:
   - event is **not** a pull request, and
   - branch is the repository **default branch**.

This prevents PR branches from deploying to production.

## Local preview

Run locally from repo root:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.
