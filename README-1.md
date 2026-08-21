# Ishita Biswas — Portfolio

A single-page portfolio site for Ishita Biswas, Content Strategist & Independent Product Builder.

**Live site:** https://ishitabiswas0201-lab.github.io

## What's in this repo

- `index.html` — the entire site (HTML, CSS, and Google Fonts import all in one file)
- `resume.pdf` — downloadable résumé, linked from the "Download résumé" buttons on the page

No build step, no dependencies, no framework. It's plain HTML/CSS that runs anywhere a static file can be served.

## Deploying

### Option A — GitHub Pages (matches the current `github.io` URL)

1. Create a GitHub repo named exactly `ishitabiswas0201-lab.github.io` (this special name makes GitHub serve it at the root domain).
2. Add `index.html` and `resume.pdf` to the repo root.
3. Push to the `main` branch:
   ```bash
   git init
   git add index.html resume.pdf
   git commit -m "Deploy portfolio"
   git branch -M main
   git remote add origin https://github.com/ishitabiswas0201-lab/ishitabiswas0201-lab.github.io.git
   git push -u origin main
   ```
4. In the repo, go to **Settings → Pages**, confirm the source is set to the `main` branch, root folder.
5. Site goes live at `https://ishitabiswas0201-lab.github.io` within a minute or two.
6. To update later: edit `index.html` locally, then `git add`, `git commit`, `git push` again — it redeploys automatically.

### Option B — Netlify (no GitHub required)

1. Go to [netlify.com](https://app.netlify.com) and log in (or sign up free).
2. Drag the folder containing `index.html` and `resume.pdf` straight onto the Netlify dashboard's deploy area.
3. Netlify uploads it and gives you a live URL immediately (e.g. `random-name-123.netlify.app`).
4. Optional: in **Site settings → Change site name**, pick a custom subdomain.
5. To update later: just drag the folder onto the dashboard again — no CLI or Git needed.

Both options are free for a static site like this.

## No README needed?

If you'd rather skip having a README in the repo at all, that's completely fine — GitHub Pages and Netlify don't require one; they just serve whatever `index.html` they find. A README only helps future-you (or anyone else) remember what the project is and how to redeploy it.
