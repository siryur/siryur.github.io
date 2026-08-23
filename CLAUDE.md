# Repo guide for AI agents

This is the source for a static, single-page site published via GitHub
Pages at siryur.com. It is a public skills portfolio for the "siryur"
handle — not a personal blog or resume with identifying details.

## Hard rules

- Never add a real name, employer, client, or other personally
  identifying information anywhere in this repo (content, commit
  messages, filenames, comments).
- Never commit secrets, API keys, or credentials.
- Content stays scoped to skills, working approach, and general
  technologies — not specific past experiences, dates, or companies.
- This file itself is public. Don't add anything here you wouldn't
  want published.

## Structure

- `index.html` — all page content (single page, no templating)
- `styles.css` — styling, theme-aware via `prefers-color-scheme`
- `robots.txt`, `sitemap.xml` — crawler config
- `CNAME` — custom domain (siryur.com)

There is no build step, framework, or package manager. Keep it that
way unless there's a concrete reason to add one.

## Local preview

```
python3 -m http.server 8000
```
then open `http://localhost:8000/index.html`.

## Deploy

GitHub Pages is configured on the legacy Jekyll build, source =
`main` branch, path `/`. Merging to `main` deploys automatically —
there is no GitHub Actions workflow and none is needed for this
setup.

## Conventions

- Keep commits small and focused; don't bundle unrelated changes.
- Subject line ≤ 50 chars, imperative mood, body wrapped at 72 chars
  if needed.
- Don't reference AI assistants in commit messages (no
  "Co-Authored-By" trailers, no "Generated with ..." lines).
- Before adding new content, check it against the hard rules above.
