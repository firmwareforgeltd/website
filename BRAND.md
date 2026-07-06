# FirmwareForge Ltd — Brand Guide

**Tagline:** Code. Hardware. Impact.
**Feel:** engineering-grade, dark, precise, warm accents — a forge, not a startup gradient.

---

## Colours

### Core palette

| Name | Hex | RGB | CMYK (print approx.) | Use |
|---|---|---|---|---|
| **Forge Orange** | `#F0751D` | 240 117 29 | 0 / 60 / 92 / 0 (≈ Pantone 158 C) | Primary accent: CTAs, links, logo anvil face, highlighted words, punctuation dots |
| **Ink** | `#1A222C` | 26 34 44 | 78 / 64 / 48 / 62 | Logo body, nav/panel backgrounds, dark text on light |
| **Page** | `#10161D` | 16 22 29 | — | Website page background |
| **Off-white** | `#F5F7F9` | 245 247 249 | 3 / 1 / 1 / 0 | Logo body on dark backgrounds, light surfaces |

### Supporting (web)

| Name | Hex | Use |
|---|---|---|
| Orange Hover | `#FF8A33` | Hover state for orange buttons/links |
| Card | `#161E27` | Card backgrounds on Page |
| Line | `#26313D` | Borders, dividers, outlines |
| Text | `#F2F5F7` | Body text on dark |
| Text Dim | `#A7B2BE` | Secondary text on dark |
| Slate | `#3A4552` | Tagline / secondary text on light backgrounds |

**Rules**

- Orange is an *accent*, never a background for large areas (buttons and small blocks only).
- On dark backgrounds, body text is Text/Text Dim — never pure white `#FFFFFF`.
- Full stops in "Code. Hardware. Impact." and headline-ending periods are always orange.

### CSS tokens

```css
:root {
  --orange: #F0751D;
  --orange-hover: #FF8A33;
  --bg: #10161D;
  --bg-panel: #1A222C;
  --bg-card: #161E27;
  --line: #26313D;
  --text: #F2F5F7;
  --text-dim: #A7B2BE;
}
```

---

## Typography

**Typeface:** [Inter](https://rsms.me/inter/) everywhere (Google Fonts on web; installed locally for design work).
Fallback stack: `"Inter", system-ui, -apple-system, "Segoe UI", Roboto, sans-serif`.
Code / part numbers: `ui-monospace, monospace`.

| Role | Weight | Notes |
|---|---|---|
| H1 / hero | 800 | letter-spacing `-0.03em`, line-height 1.1 |
| H2–H3 | 700 | letter-spacing `-0.02em`; H2s may be prefixed `// ` in orange |
| Body | 400 | line-height 1.6 |
| Nav, labels | 500–600 | |
| Buttons | 600 | |
| Tagline | 600 | UPPERCASE, letter-spacing `0.22em` |

**Wordmark:** "Firmware" in Ink (Off-white on dark) + "Forge" in Forge Orange, Inter 700, letter-spacing `-0.02em`, with a small superscript "Ltd." at weight 600.

---

## Logo

Assets live in `firmwareforge-logo/` (print-safe outlined SVGs at top level, editable Inter-text sources in `src/`, raster exports in `png/`).

| File | Use |
|---|---|
| `logo-icon.svg` | Icon, light backgrounds |
| `logo-icon-dark.svg` | Icon, dark backgrounds (also the site favicon) |
| `logo-horizontal.svg` | Full lockup, light backgrounds |
| `logo-horizontal-dark.svg` | Full lockup, dark backgrounds |

**The mark:** an anvil forming a letter F — orange anvil face on top, Ink body, three orange circuit traces terminating in node rings on the left.

**Rules**

- Clear space: keep at least the height of the orange anvil face free on all sides.
- Minimum sizes: icon 24 px, horizontal lockup 140 px wide.
- Don't recolour, outline, rotate, add effects, or place the Ink-body version on dark backgrounds (use the `-dark` variants).
- For print, use the top-level SVGs (text already outlined) and convert to CMYK using the values above.

---

## Graphic language

- Circuit-trace motifs: thin (2–2.5 px) orange lines with right-angle bends and small circular via nodes, at low opacity (~15%) as background texture, ~55% for foreground detail.
- Icons: 2 px stroke, rounded caps, single colour (orange on dark).
- Cards: `--bg-card` fill, 1 px `--line` border, 12 px radius; border turns orange on hover.
- Buttons: orange fill, white text, 8 px radius.

---

## Voice

- Plain-spoken engineering: "products that just work", not "synergistic solutions".
- UK English (colour, specialise).
- Short declaratives with orange full stops for emphasis: *Built to last.*
