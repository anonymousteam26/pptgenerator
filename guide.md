# LVMH MRI Presentation Style Guide
*For Claude (or any AI tool) to build on-brand decks without needing the original template files.*

Verified directly against both source templates' XML (`20240918_LVMH_MRI_PPT_Template_vPro.pptx` and the ABM deck) — both share the exact same theme, palette, and slide size, so this guide applies to either.

---

## READ THIS FIRST — Mandatory Build Sequence

This is not reference material to skim for inspiration. It is a spec to follow exactly. Do not substitute your own default styling, palette, layout habits, or font choices at any point below. If something isn't covered here, ask rather than improvise.

**Before writing any content:**
1. **Fetch this guide in full**, and fetch every image URL referenced in Section 10 that you intend to use. If you cannot fetch a URL (no browsing/fetch capability in this tool), say so explicitly and ask the user to paste the content or attach the files directly — do not proceed and silently skip images.
2. **Do not default to a generic "title + bullet list" template repeated on every slide.** This is the single most common failure mode. For *every single slide*, explicitly pick one named layout family from Section 8 based on what that slide needs to do. A deck where every slide uses the same layout has failed this spec, even if the colors and fonts are correct.
3. **Do not place the logotype image and the header text lockup in the same place.** See Section 4 — the top-right corner is text only, always. The logo SVGs in Section 10 are a separate asset for separate, occasional use (see Section 10 rules). Never both in the same spot.
4. **Decorative photography is a full-bleed background, never a small inset next to a text card.** See Section 7 for the one narrow exception (actual diagrams/screenshots that are themselves the content).
5. Apply the font, color, and alignment rules in Sections 2–4 exactly — including on furniture (kicker, footer, page number), not just titles.
6. Validate against the checklist in Section 11 before presenting the file.

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

Do not introduce colors outside this list.

---

## 3. Typography

**Font:** LVMH (proprietary, not available outside the original template). Fallback rule — **not optional, apply exactly:**

| Element | Font |
|---|---|
| Cover/display title, slide titles, quote pull, stat numbers, body text | **Bodoni MT** |
| Kicker label (small top-left section tag) | Calibri |
| Footer text + page number | Calibri |

Bodoni MT is used almost everywhere on purpose — it's the closest safe match to the proprietary LVMH typeface's high-contrast serif character, and it ships with Microsoft Office so it's reliably available. Only the kicker and footer stay in Calibri, because they're small, dense, utilitarian text where a Didone serif hurts legibility.

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

## 4. Recurring Furniture (every slide) — including alignment

Verified directly against the template XML across every layout family (Cover, Content, Chapter, Summary, Quote, Agenda) — these are identical across all of them, not layout-specific.

**Header, top right — TEXT ONLY, never combine with the logo image:**
"LVMH / MEDIA RESEARCH / & INSIGHTS" — x=11.85, y=0.18, w=1.3, h=0.85 — Calibri 7pt bold, **right-aligned**, Navy, 9pt line spacing.
This is the only thing that goes in this corner. The logotype SVG (Section 10) is a different asset for different, occasional placements — see Section 10's rules on when to use it. If you use the logo image, it does not also get this text next to it in the same corner.

**Kicker label, top left:**
x=0.55, y=0.26, w=10, h=0.22 — Calibri 8pt bold, Slate, +2 tracking, ALL CAPS, **left-aligned**.
The template's own built-in default text is **"SECTION 001"** (verified in the layout XML). Past decks have also used a "0N — LABEL" convention (e.g. "01 — MVP MINDSET"), which works equally well — pick one convention and stay consistent within a single deck rather than mixing both.

**Footer text:** "STRICTLY CONFIDENTIAL – INTERNAL USE ONLY – LVMH MRI" — x=0.274, y=7.1, w=10, h=0.2 — Calibri 7pt, Light Grey, **left-aligned**.

**Page number:** x=12.6, y=7.1, **right-aligned**.

**Cover/title slide title:** **centered**, both horizontally and vertically within its text box.

**Content/Chapter/Summary/Quote-Left/Quote-Right slide titles:** **left-aligned**. (For Quote-Left/Right, "Left/Right" describes which side of the slide the whole quote block sits on — the text inside that block is still left-aligned, not centered or right-justified.)

**Quote-Centered layout only:** title/quote pull is **centered**.

**Body text and bullets:** **left-aligned**, always.

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

## 7. Images: Backgrounds vs. Content — this distinction matters

There are two completely different categories of image, and they're used differently. Do not treat them the same way.

**A. Decorative/mood photography** (the texture photos, tree/fish/robot-hand style images in Section 10's backgrounds folder) — **always used as a full-bleed background image**, with a color/luminance overlay if text sits on top of it (see Section 2's note on color variants). **Never** placed as a small inset picture next to a text card. This is the single most common mistake — if a slide has a text card *and* a decorative photo in a box beside it, that's wrong; the photo belongs behind the whole slide, not boxed next to the text.

**B. Diagrams, screenshots, charts — actual content that happens to be an image** (e.g. a screenshot of a table, an existing diagram with its own embedded text/labels) — these are not decorative background material, and putting a dark color overlay behind them would make them illegible. These are the one legitimate case for the "text card + inset image" composition:

**Concept + Evidence** (single topic, one supporting diagram/screenshot)
Text card ~55–60% width on the left (Concept / Applied / Framework structure), image right, ~0.4" gap between. Use this *only* for actual reference diagrams/screenshots, never for decorative photography.

**B2. Two-Panel Comparison**
Two equal-width cards side by side (e.g. Cream left / Dark Blue right), each with its own header + bullet list. Good for cost breakdowns, before/after, options A vs B. No photography involved.

**B3. Numbered Process Flow**
N circles (Navy fill, white bold number), evenly spaced, connected by a thin Light Grey horizontal line; short caption (bold label + one line of detail) centered below each circle. Good for pipelines, sequences, timelines.

**B4. Quote**
Use the template's own dedicated `QUOTE Centered/Left/Right` layouts (Section 8) directly — don't rebuild from scratch.

---

## 8. Layout Catalog (main template — 150 named layouts)

**This is the part most likely to get skipped — don't skip it.** A generic AI-generated deck defaults to one repeated layout (title + bullets) for every slide. This template has real structural variety, verified directly against the XML geometry below — not just different colors on the same shape. Every slide should be a conscious choice from this catalog, and a deck should visibly use more than one or two families.

### COVER
Title centered both ways in a box roughly 9.84"w × 0.75"h, positioned starting ~1.75" from the left edge (so it reads as centered on the full slide). Variants: GIF Full Screen, GIF Title+Logo, STATIC × 4 colors (Dark Blue/Blue/Light Blue/Gradient — same base photo, different overlay per Section 10).

### CONTENT
Title left-aligned near the top (~24pt). Below it: a thin subtitle line (template's own placeholder prompt: "CLICK TO EDIT SUBTITLE"), then one large body placeholder spanning nearly the full width — this is the one you manually split into columns/cards yourself (see Section 8's gotcha note below). Kicker default text in the template is **"SECTION 001"** — you can use this literal convention, or the "0N — LABEL" convention already established in past decks; either is acceptable, just be consistent within one deck.

### CHAPTER (section divider)
Minimal by design: a title text block plus a subtitle line directly beneath it, positioned roughly a third of the way down the slide (title ~y=2.76", subtitle right below). No body content area — this is meant to be a clean breather slide between sections, not a content slide. Don't add bullets here; if you have real content, use CONTENT instead.

### SUMMARY
A genuine **split-panel layout**, not just a recap list: left ~40% of the slide is a solid Navy panel holding just a short title ("Add a title there" — keep it brief, it's a narrow column); the right ~60% holds a **2-column × 4-row numbered grid** (8 short items total, each with a "00" number label and a text line) — this is a real structural grid, not prose. Good for an 8-point agenda/recap; don't try to force long sentences into these cells.

### QUOTE
Three positional variants, each in 4 colors:
- **Centered:** quote text and attribution both centered in a ~7.84"-wide box, symmetric margins (~2.75" each side). Attribution sits directly below the quote, small gap.
- **Left / Right:** the same quote+attribution block, but the whole block shifts to sit in the left or right half of the slide — text inside the block stays left-aligned (not centered, not right-justified) even in the "Right" variant. Use Left/Right when you want the opposite half of the slide to breathe (e.g., paired with a portrait photo or the dark/light split treatment in Section 6).

### AGENDA (3) / (4) / (5) / (6)
An evenly-spaced row of N columns (3, 4, 5, or 6 depending on which family), each column = a large label + a small all-caps sub-label beneath it, e.g. a numbered agenda item and its short description. Each family comes in 4 colors × a set of **"Part 0, Part 1, Part 2..." variants** — these aren't different content, they're the *same* agenda slide repeated once per item, with one column's text color inverted (light-on-dark background becomes dark-on-light, or vice versa) to visually highlight "we are here" as you click through the deck. Use consecutive Part slides as a walkthrough, one per agenda item, not just a single static agenda slide.
A "Multi Image" variant exists per family/part — in the blank template this doesn't come with real per-item photos already placed, so if you want a photo per agenda item, you'll need to add picture elements yourself sized to match the column layout; don't assume the layout auto-populates images.

### AGENDA VERTICAL (4) / (5)
Same column-and-highlight logic as AGENDA, rotated to a vertical stack instead of a horizontal row. Use when there are more items than comfortably fit horizontally, or the content reads more naturally top-to-bottom.

### IMAGE DUO / TRIO
Full-bleed decorative image dividers (2 or 3 photos side by side, no color overlay by default). **Not** for readable text-bearing screenshots — there's no dark overlay to guarantee small text stays legible over busy photography. Use for mood/section breaks with minimal or no text, not for diagrams (see Section 7's A/B distinction).

### TOOLBOX
Colors, Filters, Devices, Icons, Logotype — these are the template's own internal reference/asset sheets, not slides to present. This is where the actual logo SVGs (Section 10) came from.

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

**When to actually use the logo files — this is rare:** the top-right text lockup (Section 4) is the default brand mark on every single slide, and that's usually sufficient. Only use the standalone logo SVG when a slide has no top-right text lockup at all and specifically needs a standalone mark — e.g. a divider/closing slide built as a full-bleed image with no furniture text, or an external-facing cover. If a slide already has the header text lockup, it does not also need the logo image. Never place both in the same corner.

**Path convention once in the repo:**
- `[repo-url]/assets/backgrounds/...`
- `[repo-url]/assets/logo/...`

**Adding more images going forward:** extract directly from the source `.pptx` (rename to `.zip`, unzip, images are in `ppt/media/`), filter out icons/duplicates/non-photo files, and drag straight into the local repo folder via GitHub Desktop. No need to route new images through Claude — just update this guide's inventory list afterward so Claude knows what's newly available.

---

## 11. Build Checklist — validate before presenting the file

1. Did you fetch every asset URL you intended to use? If any failed, did you say so rather than silently omitting it?
2. Does every slide use a deliberately-chosen layout family from Section 8 — not the same generic layout repeated throughout?
3. Is every title/kicker/footer/page-number aligned per Section 4 — cover title centered, everything else left, footer/page-number right?
4. Is Bodoni MT applied to titles/body/quotes/stats, and Calibri only on the kicker and footer?
5. Is any decorative photography used as a full-bleed background (never boxed next to text)? Are actual diagrams/screenshots (not decorative photography) the only things in an inset/card position?
6. Does the top-right corner contain either the text lockup OR the logo image — never both?
7. Is every color used actually in the Section 2 palette — nothing invented?
8. No leftover placeholder text, all images resolve, file opens cleanly.
