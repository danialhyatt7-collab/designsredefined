# Designs Redefined — X

A Higgsfield-styled rebuild of the Designs Redefined site: same visual language, same
sales architecture, applied to a web design and marketing studio.

Single self-contained `index.html`. No build step, no dependencies.

## Design system lifted from higgsfield.ai

| Token | Value | Where it came from |
| --- | --- | --- |
| Accent | `#d1fe17` (acid lime) | `--color-btn-accent-bg` / `--color-font-brand` |
| Accent text | `#131517` | `--color-btn-accent-text` |
| Secondary | `#ff005b` (hot pink) | `--color-font-brand-secondary` |
| Tertiary | `#9ce6f3` (ice cyan) | `--color-brand-tertiary` |
| Base surface | `#131517` / `#0e1011` | `--color-button-primary`, black scale |
| Text ramp | `#fff` → `rgba(255,255,255,.70/.45/.28)` | `--color-font-primary/secondary/tertiary` |
| Hairlines | `rgba(255,255,255,.08/.14)` | `--color-divider-primary/secondary` |
| Display font | Space Grotesk 300–700 | `/fonts/space-grotesk/space-grotesk-latin-300-700.woff2` |
| Body font | Inter 100–900 | `/fonts/inter/inter-latin-100-900.woff2` |

Effects reproduced: conic-gradient hairline card borders (`--es-border-gradient-card`),
the radial dot pattern (`--es-dot-pattern`), glass blurred nav, radial brand glows,
horizontal snap rails with drag-to-scroll, hover lift + image scale, infinite marquee,
gradient-clipped headline text.

## Sales and upsell strategy lifted from higgsfield.ai

Higgsfield monetises through a fairly specific funnel. Each move is mapped to an
agency equivalent here:

| Higgsfield move | Applied as |
| --- | --- |
| Permanent "Pricing 30% OFF" badge in nav | Nav badge + top announcement bar, same discount framing |
| Deadline and prize-pool scarcity (festival, Sept 3) | "Summer sprint" discount + a live monthly build-slot counter |
| Free tier as top of funnel | Free site audit, kept even if you never hire |
| Three consumer tiers (Basic / Pro / Max) | Launch / Growth / Scale, middle tier flagged "Most chosen" |
| Annual toggle showing % saved | One-off vs monthly-partner toggle showing "SAVE 22%" |
| Anchor pricing (struck-through original) | `was` price struck through on every tier |
| Credit add-ons and top-ups | Eight à-la-carte add-ons (care, motion, SEO, rush, copy, photo, ads, pages) |
| Team / Scale seat plans | Agency and white-label partnering strip |
| Enterprise "talk to sales" path | Scale tier and partnering CTA both route to a call, not a cart |
| Preset gallery, every tile a CTA | Twelve style directions, each tile a "Use this →" entry point |
| Community project showcase | Live client work, opened in the wild rather than as mockups |
| Cross-sell rail of adjacent products | Featured rail: 7-Day Site, Motion Pack, Audit, Store Build, Site Care |
| Persistent upgrade prompt | Sticky offer bar after the hero, dismissible per session |

Everything downstream of the hero ends in the same two actions: book the audit, or
start a project.

## Local preview

```
python3 -m http.server 8000
# open http://localhost:8000/x/
```
