# Claire Landing Page

A clean, modern static marketing site for **Claire** — Cirruslabs' AI employee platform.

## Stack

- **Vite 5** — build tool and dev server
- Plain **HTML + CSS** — no JS framework; keeps the bundle minimal
- Design tokens in `tokens.css` — single source of truth for all values
- CI via **GitHub Actions** — lint + Vite build on every push and PR

## Quick start

```bash
npm ci          # install
npm run dev     # dev server → http://localhost:5173
npm run build   # production build → dist/
npm run preview # preview the production build locally
npm run lint    # ESLint
```

## Environment variables

None required for the static site. Add a `.env` file (gitignored) for any future
analytics or API keys — see `.env.example` when one is added.

## Project layout

```
claire-landing/
├── index.html          # Entry point — sections filled in by S-4
├── tokens.css          # CSS design tokens (S-2) — source of truth
├── styles.css          # Component styles (S-4)
├── vite.config.js      # Vite configuration
├── eslint.config.js    # ESLint flat config
├── package.json
├── DESIGN.md           # Visual direction, palette, type scale, motion (S-2)
└── .github/
    └── workflows/
        └── ci.yml      # Lint + build on push / PR
```

## Sections (implemented in S-4)

1. **Hero** — headline, sub-headline, primary CTA
2. **Features** — 4 capability cards
3. **Trust bar** — credibility signals
4. **CTA band** — "Book a demo"
5. **Footer**

## Design

See [`DESIGN.md`](./DESIGN.md) for the full visual direction, token reference and assumptions.

## Assumptions

See `DESIGN.md` § Assumptions. All brand/copy assumptions are labelled; none are verified facts.
