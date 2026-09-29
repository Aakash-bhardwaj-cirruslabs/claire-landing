# Claire — Design Direction

## Direction: "Calm Authority"

Inspired by Linear, Vercel and Stripe's enterprise aesthetic — deep, confident surfaces with a single electric accent. Not cold or grey-lifeless: the Indigo accent and Coral signal give it warmth and urgency exactly where they're needed.

---

## Reference
Cirruslabs brand: deep navy, enterprise-serious, "bold but responsible, technically credible, no hype."
Claire extends that with an AI-product identity: precise, capable, human-adjacent.

---

## Typeface
**Inter** — variable font loaded from Google Fonts.  
No fallback serif; system-ui stack as the CSS fallback only.

### Type Scale (px → rem @ 16px base)
| Token              | Size   | Weight | Use                        |
|--------------------|--------|--------|----------------------------|
| `--text-xs`        | 12px   | 400    | Captions, legal            |
| `--text-sm`        | 14px   | 400    | Secondary body, labels     |
| `--text-base`      | 16px   | 400    | Body copy                  |
| `--text-lg`        | 20px   | 500    | Lead / intro               |
| `--text-xl`        | 24px   | 600    | Section headings           |
| `--text-2xl`       | 32px   | 700    | Sub-hero headings          |
| `--text-3xl`       | 48px   | 800    | Hero headline (desktop)    |
| `--text-4xl`       | 64px   | 800    | Hero headline (wide)       |

---

## Colour Palette

### Brand
| Name            | Hex       | Use                                      |
|-----------------|-----------|------------------------------------------|
| Claire Indigo   | `#4F46E5` | Primary accent — CTAs, focus rings, links |
| Indigo Light    | `#818CF8` | Hover states, decorative tints           |
| Midnight Ink    | `#1E1B4B` | Hero background, darkest surface         |
| Signal Coral    | `#FB7185` | Secondary accent — badges, highlights    |
| Mint Pulse      | `#34D399` | Success states, "live" indicators        |

### Neutrals (light mode)
| Token                | Hex       | Use                          |
|----------------------|-----------|------------------------------|
| `--surface-0`        | `#FFFFFF` | Page / card background       |
| `--surface-1`        | `#F8FAFC` | Subtle section fill          |
| `--surface-2`        | `#F1F5F9` | Input background, dividers   |
| `--border`           | `rgba(15,23,42,0.10)` | 1px borders          |
| `--text-primary`     | `#0F172A` | Body text (≥ 4.5:1 on white) |
| `--text-secondary`   | `#475569` | Muted / secondary text       |
| `--text-tertiary`    | `#94A3B8` | Captions, placeholders       |

### Neutrals (dark mode)
| Token                | Hex       | Use                          |
|----------------------|-----------|------------------------------|
| `--surface-0`        | `#0F172A` | Page background              |
| `--surface-1`        | `#1E293B` | Card / panel background      |
| `--surface-2`        | `#334155` | Input background             |
| `--border`           | `rgba(255,255,255,0.10)` | 1px borders        |
| `--text-primary`     | `#F8FAFC` | Body text                    |
| `--text-secondary`   | `#94A3B8` | Muted                        |
| `--text-tertiary`    | `#475569` | Captions                     |

### Hero Gradient
```
linear-gradient(135deg, #1E1B4B 0%, #312E81 45%, #1E1B4B 100%)
```
A subtle diagonal sweep from Midnight Ink through deep Indigo and back — depth without noise.

---

## Spacing Scale (4px base)
`4 · 8 · 12 · 16 · 24 · 32 · 48 · 64 · 96 · 128`

---

## Radii
| Token          | Value  | Use                         |
|----------------|--------|------------------------------|
| `--radius-sm`  | 6px    | Badges, tags                |
| `--radius-md`  | 10px   | Buttons, inputs             |
| `--radius-lg`  | 16px   | Cards, panels               |
| `--radius-xl`  | 24px   | Feature hero cards          |
| `--radius-full`| 9999px | Pills, avatars              |

---

## Elevation
| Level | Value                                        | Use           |
|-------|----------------------------------------------|---------------|
| 0     | none                                         | Flat surfaces |
| 1     | `0 1px 3px rgba(0,0,0,.08), 0 1px 2px rgba(0,0,0,.06)` | Cards |
| 2     | `0 4px 16px rgba(0,0,0,.12), 0 2px 4px rgba(0,0,0,.08)` | Modals, dropdowns |

---

## Motion
- **Duration:** 200ms (micro), 300ms (transitions)
- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)` (ease-in-out)
- **Hover:** 200ms ease-out on colour, transform, shadow
- **Reduced motion:** all transitions suppressed via `prefers-reduced-motion: reduce`

---

## Control Heights
| Size | Height | Use                      |
|------|--------|--------------------------|
| sm   | 32px   | Compact / inline         |
| md   | 40px   | Default buttons, inputs  |
| lg   | 48px   | Hero CTAs                |

---

## Layout
- Max-width content container: **1280px**, centred, `padding: 0 24px`
- Mobile breakpoint: **640px**
- Tablet breakpoint: **1024px**

---

## Icon Set
**Lucide** — consistent 20px / 24px stroke icons throughout.

---

## Assumptions
1. No Figma file connected — tokens derived from Cirruslabs brand research + S-1 story.
2. Inter loaded via Google Fonts; self-hosting is a future optimisation.
3. Dark mode is `@media (prefers-color-scheme: dark)` — no manual toggle in v1.
