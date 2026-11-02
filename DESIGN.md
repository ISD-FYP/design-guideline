---
version: v4
name: Dog-Diary-design-guideline
description: "Dog Diary's design language, measured 2026-11-01 from the two live decks — Dog Diary.pptx (3-slide concept sample) and Dog Diary Midterm.pptx (16-slide working deck). A flat warm-paper editorial system: cream canvas FAF7F1, sage-green ink, one terracotta accent, white hairline cards with sharp corners, Fraunces serif voice with Avenir Next working text, soft caramel/sage illustrations on cover, closing, and two content pages."
canvas:
  size: 20 x 11.25 in        # both decks are Canva exports (1920x1080 @96dpi)
  powerpoint: 13.33 x 7.5 in # divide every pt / in below by 1.5 when rebuilding in PowerPoint
palette:
  colors:
    # — midterm working system (canonical) —
    paper: FAF7F1            # every slide, flat fill — warm near-white cream
    card: FFFEFB             # all cards, near-white
    hairline: E3D9C8         # 0.75pt card border — the only standard border
    ink: 3F5246              # Fraunces: titles, card heads, hero, statements
    body: 4F5B50             # Avenir body text, sage-gray
    mute: 8A7C6E             # month ruler, quiet labels — taupe, not green
    terracotta: C05B2E       # the one loud color: eyebrows, numbers, emphasis, final bar
    terracotta-deep: B4653C  # closing thank-you line only
    apricot-tint: F4E2D4     # tint fill for callout cells and optional nodes
    sage: 7E8C6D             # connectors, timeline bars, secondary node border
    espresso: 2D251E         # arch node titles, darkest border accent
    night-line: 5A4F45       # day-strip LEAVES/RETURNS text, mute brown
  brand-layer:               # 3-slide concept sample (Dog Diary.pptx) — origin of the look
    paper-texture: F8F0E5    # full-page cream paper texture (asset assets/paper-texture.png; page 2 reads FBF5EB)
    apricot-num: CB7B4F      # giant stat numbers in the sample
    apricot-tag: D18351      # taglines (variant D18353 measured)
    ink-variants: [3D5242, 41544B]
    sage-panel: B1B696       # big sage texture panel (asset assets/sage-block.png; reads 9EA77F-B1B696)
    sage-illust: [BABDA7, 8B9481]   # hardware illustration tones
    caramel: [D9B481, E4C597, 958259] # cover dog illustration tones
    sage-scene: [AAB08E, F2EBDB, 586754] # cream dog on rounded sage panel (asset assets/dog-illustration-sage.png)
typography:
  display-serif:
    role: hero, slide titles, card heads, numbers, statements — the diary's voice
    deck: Fraunces Bold      # as exported by Canva ("Fraunces Bold")
    web: "Fraunces, Georgia, Cambria, 'Times New Roman', serif"
    pptx-fallback: Cambria Bold   # Office-shipped metric-safe stand-in
  body-sans:
    role: body, labels, node titles, captions
    deck: Avenir Next        # exported as "Avenir Next Arabic" (Canva quirk)
    web: "'Avenir Next', 'Nunito Sans', 'Segoe UI', -apple-system, sans-serif"
    pptx-fallback: Calibri
  sample-deck: Boston Angel (serif) + Open Sauce (sans) — the concept sample's own pair; superseded by Fraunces/Avenir for new slides
  scale:                     # pt at native 20 x 11.25in canvas → ÷1.5 for 13.33 x 7.5in
    hero: 96pt               # cover, two lines ("Dog / Diary") → 64pt
    closing-hero: 54pt       # closing statement → 36pt
    slide-title: 46.5pt      # content-slide masthead → 31pt
    statement: 34.5pt        # two-line mid-slide declaration (slide 7) → 23pt
    stat: 37.5pt             # terracotta card numbers ("01", "451,000+") → 25pt
    card-title: 24pt         # serif card heads — the serif reaches card level → 16pt
    closing-accent: 28.5pt   # "Thank you" line, terracotta-deep → 19pt
    node-label: 18.75pt      # Avenir Bold caps, arch node titles → 12.5pt
    day-marker: 18pt         # Avenir Bold, day-strip times → 12pt
    cover-update: 20.25pt    # closing-slide update text → 13.5pt
    body: 15pt               # → 10pt
    eyebrow: 15pt bold caps, terracotta, +2.4pt tracking → 10pt, +1.6pt
    caption: 15pt caps +2.4pt, mute (month ruler) → 10pt
rounded:
  card: 0                    # sharp corners everywhere — no roundRect in either deck
  pill: none                 # no pills; even emphasis is a border or tint, never a chip
spacing:                     # native 20 x 11.25in → ÷1.5 for PowerPoint
  margin-left: 1.15in        # → 0.77in
  eyebrow-y: 0.71in          # → 0.47in
  title-y: 1.30in            # → 0.87in
  content-top: 2.7in         # → 1.8in
  card-gap-x: 0.31in         # two-card row → 0.21in
  card-gap-grid: 0.36-0.41in # 2x2 grids → 0.24-0.27in
  card-padding: 0.33in left, 0.39in top  # → 0.22 / 0.26in
  card-2col: 4.48 x 2.19in   # → 2.99 x 1.46in
  card-grid: 5.21 x 2.40in   # → 3.47 x 1.60in
elevation: none              # flat — 0.75pt hairline border, no shadows, no gradients
imagery: >
  Soft painterly illustrations with transparent backgrounds, never photos (a photo
  pass was tried and rejected). Caramel-tan dog (assets/dog-illustration.png) fills
  the right 47% full-height of cover and closing; sage hardware illustrations
  (assets/illu-camera.png, assets/illu-wearable.png) sit as right-column blocks on
  the market and feasibility pages. 4 of 16 slides carry art; the rest are type on paper.
  Brand layer keeps a second dog treatment — cream dog on a rounded sage panel
  (assets/dog-illustration-sage.png, sample-deck problem page, high-res variant) —
  the source of the sage-scene tones AAB08E / F2EBDB / 586754.
---

# Dog Diary Design Guideline

## 1. Overview

Two live decks define this system. **Dog Diary Midterm.pptx** (16 slides) is the canonical working deck — every token below is measured from its XML. **Dog Diary.pptx** (3 slides) is the concept sample that originated the look: cream paper texture, a big sage panel, giant apricot stats. The midterm reinterprets that brand in a flatter, more systematic voice: flat cream canvas, white hairline cards with sharp corners, Fraunces + Avenir Next, one terracotta accent.

Both are Canva exports at 20×11.25in (1920×1080). When rebuilding slides in PowerPoint (13.33×7.5in), divide every pt and inch by 1.5 — the scale table does this for you.

Applies to: the midterm deck (primary), the final deck, app mockups, and one-pagers. Ported to CSS tokens in `preview.html`.

## 2. Colors

Working system (midterm):

| role | token | hex | notes |
|---|---|---|---|
| canvas | paper | FAF7F1 | every slide, flat fill — warm near-white, never pure white |
| card | card | FFFEFB | all cards |
| card border | hairline | E3D9C8 | 0.75pt, the only standard border |
| display text | ink | 3F5246 | sage green — serif titles, card heads |
| body text | body | 4F5B50 | |
| quiet labels | mute | 8A7C6E | taupe; month ruler and captions |
| loud accent | terracotta | C05B2E | eyebrows, card numbers, emphasized borders, final timeline bar |
| closing accent | terracotta-deep | B4653C | one line on the closing slide |
| tint fill | apricot-tint | F4E2D4 | callout cells, optional nodes |
| system green | sage | 7E8C6D | connectors, timeline bars, secondary borders |
| darkest accent | espresso | 2D251E | arch node titles, push-node border |
| mute brown | night-line | 5A4F45 | day-strip leave/return text |

Brand layer (concept sample): paper-texture F8F0E5 / FBF5EB (asset), apricot numbers CB7B4F, apricot taglines D18351, sage panel B1B696 (asset), caramel dog D9B481 family, sage-scene dog AAB08E / F2EBDB / 586754.

Rules:

- Green is the ink (3F5246 / 4F5B50), never the background. The canvas stays cream; sage appears only in elements — connectors, bars, borders, illustration.
- Terracotta C05B2E is the single loud color. One loud moment per slide: the eyebrow is always terracotta, so anything louder (a number, an emphasized border, the final bar) is the slide's only other.
- Emphasis is a **colored border on the white card** (1.5pt terracotta/sage/espresso) or an **apricot-tint fill** — never a fill of the loud color behind text, never a chip.
- No pure white canvas, no pure black ink. Cards may be FFFEFB but the page never is.

## 3. Typography

- **Fraunces Bold speaks, Avenir Next works.** The serif carries the hero, slide titles, card heads (24pt — the serif reaches card level), numbers, and statements. The sans carries body, node labels, and captions. Never sans titles, never serif body.
- The eyebrow opens every content slide: Avenir Bold 15pt, all caps, +2.4pt tracking, terracotta — `RESEARCH`, `PROBLEM`, `ROADMAP`. It names the midterm section and keeps the deck navigable.
- Titles in sentence case, body left-aligned. Numbers always Fraunces, always terracotta, always large (37.5pt).
- Sample deck note: its own pair is Boston Angel + Open Sauce at display sizes up to 200pt (133pt at PowerPoint scale). New slides follow the midterm pair; keep the sample's gesture of letting a number run huge when it earns it.
- Deck fonts are Canva fonts. For PowerPoint regeneration use Cambria Bold / Calibri as metric-safe stand-ins; for web use the stacks in the frontmatter (Fraunces installed locally or Georgia fallback; Avenir Next ships on macOS).

## 4. Layout and spacing

- One masthead formula on every content slide: eyebrow at y=0.71in, serif title at y=1.30in, content from y=2.7in, left margin 1.15in. No rule under the title — nothing under it at all; whitespace separates.
- The cover is the only place with a mark under type: a 0.96×0.04in terracotta dash beneath the hero.
- Cards sit on the grid: two-column rows gap 0.31in, 2×2 grids gap 0.36–0.41in, card padding 0.33in left / 0.39in top. Sharp corners, 0.75pt hairline border.
- Wide statements can span the column (13in text boxes); the day-strip and timeline own the full content width.
- Nothing crosses the margins. A diary has margins.

## 5. Components

- **numbered-card** — white card, hairline border; terracotta Fraunces number ("01", 37.5pt) in the top-left, serif card head (24pt) to its right, sans body below. The deck's workhorse: principles, MVP, validation, scenario steps.
- **quote-card** — same card without the number: serif head (a quote or finding), sans body. Used in pairs or with a wide third card beneath.
- **wide-callout** — full-width card for the slide's single takeaway ("The cost of uncertainty", "The gap is not more footage"); may take apricot-tint fill when the takeaway is warm.
- **compare-cards (then/now)** — two equal cards with a wide central gap; the winning side gets the 1.5pt terracotta border, the quiet side keeps hairline.
- **day-strip** — three equal cells across the slide: LEAVES / the emphasized unknown / RETURNS. The emphasized cell takes apricot-tint fill + terracotta bold text; the others stay white with night-line text.
- **arch-node** — white card with a 1.5pt border in the node's role color (terracotta = core dog module, sage = phone, espresso = push alert); label in Avenir Bold caps (espresso) + sans sub-line; straight sage connector lines between nodes; the optional node fills apricot-tint with no border. Privacy stamps ("CLOUD OFF BY DEFAULT") are terracotta caps text, bottom-right, no box.
- **timeline** — month ruler in mute caps (+2.4pt tracking); rows of label left + sage bar (0.4in tall, square ends); the final stretch bar turns terracotta; milestones M1–M4 are terracotta caps text at bar ends, no diamonds, no circles.
- **step-row** — six narrow numbered cards telling one case start-to-finish, each with a bold time caption.
- **cover** — left column: eyebrow, 96pt two-line hero, terracotta dash, tagline, team + date in body sans. Right 47%: full-height caramel dog illustration.
- **closing** — mirror of the cover: 54pt serif statement, three white update cards, thank-you line in terracotta-deep 28.5pt, same right-half illustration.

## 6. Illustration and imagery

Soft painterly illustration with transparent backgrounds — visible brush texture, gentle gradients within one hue family. Two dog treatments: the midterm's caramel-tan dog (D9B481 / E4C597 / deep 958259) and the sample deck's cream dog on a rounded sage panel (AAB08E field, F2EBDB subject, 586754 detail — `assets/dog-illustration-sage.png`); hardware is soft sage (BABDA7 / 8B9481). No photos, no 3D, no line-icon libraries, no clip art with hard edges.

Art earns its place: cover, closing, market, feasibility — 4 of 16 slides. Everything else is type on paper. When a new slide wants art, ask what it replaces, not what it fills.

## 7. Do's and don'ts

Do:

- One loud terracotta moment per slide beyond the eyebrow
- Sharp corners, hairline borders, flat fills
- Let Fraunces carry every title, card head, and number
- Emphasize with a colored border or an apricot-tint fill
- Keep the eyebrow carrying the midterm's section names

Don't:

- Rounded corners, pills, chips — none exist in either deck
- Drop shadows, gradients, glassmorphism
- A rule or bar under content-slide titles (the cover dash is the only mark under type)
- Photos, or art on every page
- Sage text below 15pt; sage never as background
- Pure white canvas, pure black ink
