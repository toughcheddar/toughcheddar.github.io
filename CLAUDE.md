# CLAUDE.md

Guidance for Claude Code working in this repo.

## What this is

The Tough Cheddar Studios landing page. One static HTML page (`index.html`)
served by GitHub Pages at https://toughcheddar.github.io. No framework, no
build step, no dependencies — inline CSS in a single file.

## Conventions

- Keep it a single self-contained `index.html`. Don't introduce a build
  system or JS framework unless the site genuinely outgrows one static page.
- Brand colours are CSS custom properties in the `:root` block: cream
  `#f4ead2`, navy `#1d3a5f`, cheese gold `#e8a317`. Reuse them; don't
  hard-code new one-off hexes.
- Images go in `images/`. Add `loading="lazy"` and descriptive `alt` text.
  Watch file size — `tough-cheddar-alt-logo.png` is ~5 MB and is only used as
  the favicon/social image, not inlined in the page body.
- Keep copy humble and plain. The studio makes Stackpot, a card game for all
  ages. Avoid superlatives and marketing hype.

## Deploying

Pages builds from `main` root. Commit and push to `main`; the live site
updates within a minute or two. `.nojekyll` keeps Pages from running Jekyll.

## Related

- Game source / repo: https://github.com/toughcheddar/stackpot (private)
- Playable builds: https://toughcheddar.itch.io
