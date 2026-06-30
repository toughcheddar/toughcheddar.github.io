# toughcheddar.github.io

The Tough Cheddar Studios landing page. A single static HTML page served by
GitHub Pages at **https://toughcheddar.github.io**.

It introduces the studio and links out to our games on
[itch.io](https://toughcheddar.itch.io).

## Structure

```
.
├── index.html      # the whole site (inline CSS, no build step)
├── images/         # studio logo
├── .nojekyll       # serve files as-is, skip Jekyll
├── CLAUDE.md       # notes for Claude Code
└── README.md
```

## Local preview

Open `index.html` directly, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploying

Pages builds from the `main` branch root. Push to `main` and the live site
updates within a minute or two.

```bash
git add -A && git commit -m "Update site" && git push
```

## Editing

The page is intentionally a single self-contained file. Brand colours live in
the `:root` block at the top of `index.html`:

- cream `#f4ead2`, navy `#1d3a5f`, cheese gold `#e8a317`

Add new images to `images/` and reference them from `index.html`.
