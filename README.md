# Portfolio + Guides Starter (MkDocs Material + GitHub Pages)

Portable, content-first structure. Write everything in Markdown under `/content`.
Deploys to GitHub Pages via GitHub Actions.

## Write content
- Put all Markdown content in `/content`.
- Organize guides under `/content/guides/` (e.g., `sql/`, `pandas/`, `python/`).
- Portfolio items go in `/content/portfolio/` as separate pages.

## Local preview
- Install Python 3.10+
- `pip install -r requirements.txt`
- `mkdocs serve`
- Open `http://127.0.0.1:8000`

## Analytics (optional)
- **Google Analytics 4**: set `GA_MEASUREMENT_ID` in `mkdocs.yml` under `extra` → `analytics`.
- **Cloudflare Web Analytics**: uncomment the `extra_javascript` line with the Cloudflare snippet in `mkdocs.yml` and replace the token.
- **Search Console**: add your site after it’s live.

## Custom domain (optional)
- Add your domain in GitHub Pages settings and create a `CNAME` file at repo root or under `/content` if you prefer.
- Set DNS CNAME to `<your-username>.github.io.`

## Migrate later (to Next.js/Vercel)
- Keep `/content` as your single source of truth.
- A Next.js site can read Markdown from `/content` (via `gray-matter`/`next-mdx-remote`).
- No rewrites needed; only new templates.
