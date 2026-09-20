# Agent notes

Static website: hand-written `index.html` and `styles.css`, images and files in `assets/`, custom domain via `CNAME`. No build step, no tests, no package manager.

## Deployment

- Pushing to `main` deploys straight to GitHub Pages (`deploy-pages.yml`). There is no staging branch, so a push to `main` is live.

## Editing

- Content and layout changes go in `index.html` / `styles.css`; new images into `assets/`.
- Keep the existing class naming scheme rather than introducing a framework.

## Pull requests

- Base branch is `main` — this repo has no `develop`.

## Routines

Push, PR, CI and issues via `ghops`; mechanical work (renames, repeated markup changes) via `cheap-do`. Commit messages and PR bodies are generated from the diff — do not write them by hand.
