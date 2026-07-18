# fr0stm0urne.github.io

Personal website of **Muhammad Ibrahim** — Research Scientist II, CyFI Lab, Georgia Tech.

Live at **https://fr0stm0urne.github.io/**

## Stack

Plain, hand-written **HTML + CSS + JavaScript** — no Jekyll, no build step, no
dependencies, no webfonts (system monospace only). GitHub Pages serves the files
directly. Terminal / brutalist theme with a light ("paper") and dark ("green
phosphor") mode.

```
index.html            # the whole page (all sections)
assets/css/style.css  # terminal theme + light/dark tokens
assets/js/main.js      # theme toggle, mobile nav, scroll spy, reveal
assets/favicon.svg     # ">_" prompt favicon
images/profile.jpg     # portrait
files/                 # CV + paper PDFs
```

## Editing

Everything is content in `index.html`:

- **Intro / tagline** — the `.hero` section
- **Research areas** — the `.cards` in `#research`
- **Education** — the `.timeline` in `#research`
- **Publications** — the `.pub-list` in `#publications`
- **CVEs** — the `.cve-list` in `#security`
- **Contact / email / socials** — `#contact` and the hero `.socials`

Colors live as CSS variables at the top of `assets/css/style.css`
(`:root` for light, `html[data-theme="dark"]` for dark).

## Local preview

No server required — just open `index.html` in a browser. Or:

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deploy

Push to `master`. In **Settings → Pages**, source = **Deploy from a branch →
`master` / (root)**. GitHub publishes within a minute or two.
