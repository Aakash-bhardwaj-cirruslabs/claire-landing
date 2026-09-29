# Claire Landing Page

A clean, modern static marketing site for **Claire** — Cirruslabs' AI employee platform.

## Stack
- Static HTML + CSS (no framework)
- Design tokens in `tokens.css`
- CI via GitHub Actions (HTML validation + link check)

## Development

```bash
# Serve locally (any static server)
npx serve .
# or
python3 -m http.server 8080
```

## Design
See [`DESIGN.md`](./DESIGN.md) for the full visual direction, token reference and assumptions.

## Structure
```
claire-landing/
├── index.html          # Landing page (built in S-4)
├── tokens.css          # CSS design tokens — source of truth for all values
├── styles.css          # Component styles (built in S-4)
├── DESIGN.md           # Visual direction, palette, type scale, motion
└── .github/
    └── workflows/
        └── ci.yml      # HTML lint + link check
```

## Sections
1. Hero — headline, sub-headline, primary CTA
2. Features — 4 capability cards
3. Trust bar — credibility signals
4. CTA band — "Book a demo"
5. Footer

## Assumptions
See `DESIGN.md` § Assumptions.
