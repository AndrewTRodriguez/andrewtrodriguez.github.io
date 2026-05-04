# AndrewTRodriguez.github.io

This repository is configured for **GitHub Pages via GitHub Actions**.

## One-time repository setting (required in GitHub UI)

1. Open **Settings → Pages** in this repository.
2. Under **Build and deployment**, set **Source** to **GitHub Actions**.
3. Push to `main` to trigger deployment.

## Deployment workflow

The workflow file at `.github/workflows/deploy-pages.yml` publishes the repository root as a static site.
