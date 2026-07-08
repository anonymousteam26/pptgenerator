# LVMH MRI Presentation Style Guide
*For Claude (or any AI tool) to build on-brand decks without needing the original template files.*

Verified against both source templates (`20240918_LVMH_MRI_PPT_Template_vPro.pptx` and the ABM deck) — both share the exact same theme, palette, and slide size, so this guide applies to either.

---

## 0. Intake Form — fill this in before building

Copy this block, fill it in, and send it along with this guide at the start of any presentation request.

```
PRESENTATION TYPE:     [ Executive  |  Artistic ]   (see Section 0a for what each means)
AUDIENCE:              [ e.g. Katie / MAD leadership / cross-brand / external client ]
PURPOSE:               [ e.g. status update, pitch for approval, training/workshop, retro ]
LENGTH:                [ target slide count, or "let Claude decide based on content" ]
TONE:                  [ e.g. formal, conversational, persuasive, neutral/informational ]
KEY MESSAGE:           [ the one thing the audience should remember or decide ]
CONTENT SOURCE(S):     [ docs/data attached? links? or "draft from scratch based on brief below" ]
IMAGES / SCREENSHOTS:  [ do you have specific visuals to include? attach or describe ]
DEADLINE / CONTEXT:    [ when is this needed, and anything time-sensitive Claude should know ]
```

### 0a. Executive vs. Artistic — which one to pick

| | **Executive** | **Artistic** |
|---|---|---|
| Base template | Main LVMH MRI template | ABM-style template |
| Visual language | Clean, text-forward, data-driven | Full-bleed photography, bold statements, fewer words per slide |
| Layout families | `CONTENT`, `SUMMARY`, `AGENDA`, two-panel/process recipes (Section 7) | `Concept A/B` full-bleed statement slides, `QUOTE`, `Streams`/`Timeline` |
| Best for | Status updates, budget/data reviews, internal working sessions, anything with line-item detail | Kickoffs, pitches, culture/vision moments, anything meant to land emotionally in a few seconds per slide |
| Text density | Higher — cards with bullets, numbers, tables | Lower — one statement or concept per slide, image does the work |

If unsure which to pick, default to **Executive** — it's the safer, more broadly-applicable choice, and it's the one with zero embedded-object risk (see Section 9).

---



## 1. Slide Basics

- **Dimensions:** 13.333" × 7.5" (widescreen, `LAYOUT_WIDE`) — 12,192,000 × 6,858,000 EMU
- **Safe content area:** x: 0.55" → 12.8" · y: 1.1" → 6.9"
- **Font:** LVMH (proprietary) — use **Calibri** as the safe fallback in any tool that doesn't have the LVMH font installed

---

## 2. Color Palette

| Name | Hex | Usage |
|---|---|---|
| Navy | `020F2A` | Dark slide backgrounds; dominant dark color |
| Dark Blue | `0C2E56` | Card backgrounds on dark slides |
| Slate | `586170` | Muted/supporting text |
| Light Grey | `97A4AD` | Captions, footer text, divider lines |
| Cream | `F7F2EC` | Light slide backgrounds; cards on light slides |
| Gold | `ECDAA6` | Kickers on Cover/Closing slides; tag labels only — not a general accent |
| Rust | `984124` | Alerts, controversy, or a single highlighted stat — use sparingly, not as a default accent |
| White | `FFFFFF` | Content slide backgrounds |

---

## 3. Typography

| Element | Size | Weight/Style | Color |
|---|---|---|---|
| Big display title (cover) | 42–44pt | Bold | White or Navy |
| Slide title | 22–26pt | Bold | Navy `020F2A` |
| Section kicker (top label) | 8pt | Bold, ALL CAPS, +2 tracking | Slate `586170` |
| Body text | 11–13pt | Regular | Slate `586170` |
| Quote pull | 30pt | Bold, Italic | Navy |
| Stat number | 52–130pt | Bold | Navy |
| Captions / sources | 8.5–10pt | Italic | Light Grey `97A4AD` |

---

## 4. Recurring Furniture (every slide)

**Header, top right:**
"LVMH / MEDIA RESEARCH / & INSIGHTS" — x=11.85, y=0.18, w=1.3, h=0.85 — Calibri 7pt bold, right-aligned, Navy, 9pt line spacing

**Kicker label, top left:**
x=0.55, y=0.26, w=10, h=0.22 — Calibri 8pt bold, Slate, +2 tracking, ALL CAPS
*(established convention from past decks: format as `"0N — LABEL"`, e.g. "01 — MVP MINDSET")*

**Footer rule:** horizontal line, x=0.274, y=7.079, w=11.3, Light Grey, 0.5pt weight

**Footer text:** "STRICTLY CONFIDENTIAL – INTERNAL USE ONLY – LVMH MRI" — x=0.274, y=7.1, w=10, h=0.2 — Calibri 7pt, Light Grey

**Page number:** x=12.6, y=7.1, right-aligned

---

## 5. Card Style

- Shape: rounded rectangle, corner radius 0.07–0.1"
- **On light slides:** fill Cream `F7F2EC`; outer shadow (8pt blur / 3pt offset / 120° angle / 10% opacity)
- **On dark slides:** fill Dark Blue `0C2E56`
- Accent band (optional): full-width strip, 0.36–0.38" tall, top of card, in relevant accent color
- Divider lines inside cards: Light Grey, 0.4pt

**Shadow spec (reference):** outer, color `000000`, blur 8pt, offset 3pt, angle 120°, opacity 10–12%

---

## 6. Slide Structure Patterns

| Pattern | Background | Title | Cards/Content |
|---|---|---|---|
| Cover / Closing | Full Navy | White | Gold kicker |
| Content | White | Navy | Cream cards |
| Dark content | Full Navy | White | Dark Blue cards |
| Split | Left Navy / Right White | — | Gold vertical divider at x=6.0 |

---

## 7. Layout Recipes (proven patterns, not in the original templates)

These are compositions built and tested in past decks — safe to reuse directly.

**A. Concept + Evidence** (single topic, one supporting image)
Text card ~55–60% width on the left (Concept / Applied / Framework structure), image right, ~0.4" gap between. Good default for "explain one idea with one piece of visual proof."

**B. Two-Panel Comparison**
Two equal-width cards side by side (e.g. Cream left / Dark Blue right), each with its own header + bullet list. Good for cost breakdowns, before/after, options A vs B.

**C. Numbered Process Flow**
N circles (Navy fill, white bold number), evenly spaced, connected by a thin Light Grey horizontal line; short caption (bold label + one line of detail) centered below each circle. Good for pipelines, sequences, timelines.

**D. Quote**
Full Navy background, large italic Navy/White quote pull (~30pt), attribution below in Slate. *(Note: the main template already has dedicated `QUOTE Centered/Left/Right` layouts in 4 color variants — use those directly rather than rebuilding from scratch.)*

---

## 8. Layout Catalog (main template — 150 named layouts)

Full geometry for any of these can be pulled on request; this is the index of *families* so the right one gets picked without guessing:

| Family | Variants | Use for |
|---|---|---|
| `COVER` | GIF Full Screen, GIF Title+Logo, STATIC × 4 colors | Title slide |
| `SUMMARY` | 4 colors + Image Manual | Recap / agenda-style overview |
| `CHAPTER` | 4 colors | Section divider |
| `QUOTE` | Centered / Left / Right × 4 colors | Quote slides |
| `AGENDA (3/4/5/6)` | × 4 colors × "Part 0–N" (progressive highlight) | Numbered agenda with current-item highlight |
| `AGENDA VERTICAL (4/5)` | × Part 0–N | Vertical agenda variant |
| `CONTENT` | White, Dark Blue, Blue, Light Blue, Gradient | Standard text-forward slide |
| `IMAGE DUO/TRIO` | STATIC/ANIMATED × colors | Full-bleed decorative image dividers — **not** for readable text-bearing screenshots (dark overlay makes small text illegible) |
| `TOOLBOX` | Colors, Filters, Devices, Icons, Logotype | Reference/asset sheet, not a content slide |

**Known gotcha:** `CONTENT`-family slides put all body text in one full-width placeholder by default — for a text+image split, manually resize the body placeholder (e.g. to ~52% width) and add the image as a separate picture, rather than expecting a built-in two-column placeholder.

---

## 9. The Second Template (ABM deck)

Same theme/palette/fonts as above, but the file is much larger (~190MB) and several of its most visually distinctive slides (chart comparisons, some agenda slides) use **embedded chart/OLE objects**, not plain text placeholders.

**Rule: don't repurpose embedded chart objects directly** — editing around them risks corruption. Safe slides to reuse as-is: the `QUOTE` layout, simple `Concept A/B` text-on-photo statement slides, and the numbered `Streams`/`Timeline` layouts (these use plain shapes, not embedded objects).

---

## 10. Image & Logo Assets

This is a **living inventory** — small today, meant to grow as more images get added to the repo. Always check the repo's actual folder contents first, since this list will fall behind as files get added; treat it as a starting point, not a ceiling.

**Current inventory:**

*Backgrounds — Executive (from the main LVMH MRI template):*
- `lvmh-bg-01-staircase.png` — the water/staircase texture used across most Cover/Content layouts
- `lvmh-bg-03.jpeg`, `lvmh-bg-04.jpg`, `lvmh-bg-05.jpg`, `lvmh-bg-06.jpg` — additional distinct photos pulled from the template's sample slides (descriptive renames still needed — check each visually and rename to something meaningful, e.g. `lvmh-bg-04-cityscape.jpg`, once reviewed)

*Note on color variants:* the Dark Blue / Blue / Light Blue / Gradient versions of Cover/Content layouts are **not** separate image files — they're the same base photo with a color/luminance overlay on top. To recreate a color variant, apply a semi-transparent Navy or Dark Blue rectangle over the base image rather than hunting for a separate source file per color.

*Backgrounds — Artistic (from the ABM template, small sample so far):*
- `abm-tree.png`, `abm-fish.jpeg`, `abm-robothand.png` — representative photography
- (the ABM template contains far more — roughly 150+ additional usable photos not yet pulled; add in batches as needed rather than all at once)

*Logo:*
- `lvmh-logotype-black.svg` — for use on light backgrounds
- `lvmh-logotype-white.svg` — for use on Navy/dark backgrounds

**Path convention once in the repo:**
- `[repo-url]/assets/backgrounds/...`
- `[repo-url]/assets/logo/...`

**Adding more images going forward:** extract directly from the source `.pptx` (rename to `.zip`, unzip, images are in `ppt/media/`), filter out icons/duplicates/non-photo files, and drag straight into the local repo folder via GitHub Desktop. No need to route new images through Claude — just update this guide's inventory list afterward so Claude knows what's newly available.

---

## 11. Build Checklist

1. Confirm which structure pattern fits (Cover / Content / Dark Content / Split)
2. Pick the layout family from Section 8 — don't default to `CONTENT` for everything
3. Apply furniture exactly (kicker, header, footer, page number) — these should be identical on every slide
4. For text+image slides, resize the body placeholder manually; don't rely on layout defaults
5. Keep to the palette in Section 2 — no colors outside this list
6. Validate the file before presenting it (styles, no leftover placeholder text, all images resolve)
