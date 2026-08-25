# devanshpandey.github.io

Personal academic website of Devansh Pandey — live at **https://devanshpandey.github.io**.

## Structure

```
.
├── index.html           # single-page site: About, Research Interests, News,
│                        #   Research Experience, Publications, Service & Teaching
└── assets/
    ├── css/style.css    # all styling
    └── img/profile.png  # profile photo
```

## Editing

- **Add a news item**: copy an existing `<div class="news-item">` block in the
  `<section id="news">` of `index.html` and place it at the top of `news-list`
  (entries are newest-first).
- **Add a publication**: copy a `pub-item` block in `<section id="publications">`.
- Styling lives entirely in `assets/css/style.css`.

Preview locally:

```bash
python3 -m http.server 8000
```

then open http://localhost:8000.

## Deploying

The site is served by GitHub Pages from the `main` branch. Any push to `main`
goes live in about a minute:

```bash
git add -A && git commit -m "Update site" && git push origin main
```

> Note: this folder (cloned to `~/Desktop/Devanshpandey.github.io`) is the
> working copy of record. Older copies under `~/.gemini/antigravity*/scratch/`
> carry an unrelated, never-deployed git history — do not push from them.
