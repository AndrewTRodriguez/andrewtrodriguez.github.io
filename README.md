# AndrewTRodriguez.github.io

This repository is configured for **GitHub Pages via GitHub Actions**.

## Why `index.html` may not load yet

If `https://andrewtrodriguez.github.io/` is not loading, the most common reasons are:

1. **Pages source not set to GitHub Actions** in **Settings → Pages**.
2. The deploy workflow has not run successfully yet.
3. DNS/CDN propagation delay right after first publish (can take a few minutes).

## Required repository setting (GitHub UI)

1. Open **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to **GitHub Actions**.

## Deployment workflow

The workflow at `.github/workflows/deploy-pages.yml` deploys on every push and on manual dispatch.
