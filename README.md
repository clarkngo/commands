# commands

Personal command snippets with a small searchable static site for [GitHub Pages](https://pages.github.com/).

## Local preview

From this directory:

```bash
python3 -m http.server 8080
```

Open http://127.0.0.1:8080 — `commands.json` must load over HTTP (not `file://`).

## GitHub Pages

1. Push this repo to GitHub.
2. Repo **Settings → Pages → Build and deployment**: source **Deploy from a branch**, branch **main** (or your default), folder **/ (root)**.
3. After the workflow finishes, the site is at `https://<user>.github.io/<repo>/`.

## Add or edit commands

Edit `commands.json`: each entry has `title`, `command`, and optional `tags` (array of strings). Commit and push; the site updates on the next deploy.