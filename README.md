# Learning to Drive on Mars — Project Page

Static project page adapted from the [Recipe](https://toruowo.github.io/recipe/) / [HATO](https://toruowo.github.io/hato/) template.

## Preview locally

No build step — it's plain HTML/CSS. Serve the folder with any static server:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000. (A plain `open index.html` also works, but videos/CORS behave more like production under a server.)

## Customize

Everything lives in `index.html`. Search for `TODO` and placeholder text:

- **Title / authors / affiliations** — top of `index.html`.
- **Links** — arXiv id, `assets/paper.pdf`, YouTube url, GitHub repo. Delete buttons you don't use.
- **TLDR + Abstract** — the two text blocks under the title / teaser videos.
- **Media** — drop files into:
  - `results/` — `.mp4` videos (teaser carousel + result grids).
  - `figures/` — `.png` figures (`fig1.png`, `fig2.png`).
- **BibTeX** — update the citation block.
- Styling lives in `style.css`.

## Deploy to GitHub Pages

This repo publishes automatically via `.github/workflows/deploy.yml` on every push to `main`.

1. Create a repo (e.g. `learning-to-drive-on-mars`) on GitHub under your account.
2. Push this folder to it (see below).
3. In the repo: **Settings → Pages → Build and deployment → Source: GitHub Actions**.
4. Live at: `https://darren-chiu.github.io/learning-to-drive-on-mars/`

```bash
git init
git add -A
git commit -m "Initial project page"
git branch -M main
git remote add origin https://github.com/darren-chiu/learning-to-drive-on-mars.git
git push -u origin main
```
