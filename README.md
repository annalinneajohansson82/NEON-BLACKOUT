# Neon Blackout

A cyberpunk/synthwave design system on a near-black void. High-contrast neon, one spacing scale, one set of radii. Colors are mapped to the Intersex-Inclusive Progress Pride flag — every hue carries meaning.

**License:** CC0 — free to use in any project.

---

## Palette

### Surfaces

| Token | Hex | Usage |
|---|---|---|
| `--void` | `#050507` | Primary background |
| `--elev` | `#12131c` | Cards, panels, elevated surfaces |
| `--raised` | `#1a1a2e` | Transient UI only (modals, dropdowns, toasts) |
| `--fg` | `#cfc8ee` | Primary text — lavender |
| `--muted` | `#8e88ab` | Secondary text, labels, captions |
| `--line` | `rgba(207,200,238,0.14)` | Borders, dividers |
| `--line-soft` | `rgba(207,200,238,0.07)` | Subtle dividers |

### Heritage (flag → UI)

| Name | Hex | Role |
|---|---|---|
| Static Magenta | `#ff00aa` | Brand, primary action |
| Signal Cyan | `#00fff0` | Focus, cursor, active indicator |
| Lifeblood Red | `#ff3864` | Errors, destructive actions |
| Pulse Green | `#39ff14` | Success, confirmed |
| Sunlight | `#fcee09` | Warnings |
| Harmony Blue | `#00aaff` | Info, structural accents |
| Mending Orange | `#ff9f1c` | Staged, intermediate |
| Spirit Violet | `#7b3fd4` | Accent (large text only) |

### Typography

| Role | Font |
|---|---|
| Display | Audiowide |
| Body | Space Grotesk Variable |
| Mono | Space Mono (min 0.8rem) |

### Spacing scale

8px base. Tokens: `--space-4` (4px) through `--space-96` (96px). Use these for all padding, margin, and gaps — no arbitrary values.

### Border radius

| Token | Value | Usage |
|---|---|---|
| `--radius-sm` | 4px | List items, subtle corners |
| `--radius-md` | 6px | Buttons, inputs, toasts |
| `--radius-lg` | 10px | Panels, cards, elevated surfaces |
| `--radius-full` | 999px | Pills, badges |
| `.circle` | 50% + 1:1 | Avatars, indicators |

### Glow system

8 colours × 4 strengths, composable utility classes. Pattern: `.glow-{color}-{strength}` where colour is one of `magenta`, `cyan`, `blue`, `green`, `red`, `yellow`, `orange`, `violet` and strength is `sm`, `md`, `lg`, `xl`. Text variant: `.glow-text-{color}`.

---

## Files

| File | What |
|---|---|
| `dtcg-tokens.json` | Canonical DTCG token source — single source of truth |
| `tokens.json` | Human-readable token reference with ANSI mappings |
| `neon-blackout.css` | Production CSS with all tokens, glow system, component styles |
| `component-spec.html` | Visual component spec — open in a browser |
| `hermes/skins/neon-blackout.yaml` | Hermes TUI skin |

Uses `color-mix()` for background tints and `prefers-reduced-motion` / `prefers-contrast` for accessibility. WCAG 2.2 AA compliant across all interactive text pairings.

---

## Related

- **[Neon Whiteout](/home/anna/Projects/neon-whiteout)** — light-mode sister system. Same palette, inverted surfaces. Glow → Halo.
