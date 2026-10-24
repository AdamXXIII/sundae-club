---
name: Sundae Club
description: A hardware-shop paint fan deck for a co-op horror game about painting yourself into the wall.
colors:
  night: "#17142a"
  night-2: "#211d38"
  paper: "#e8eaf0"
  ink: "#17142a"
  ink-2: "#413b58"
  paper-dim: "#cfc9dc"
  sundae-pink: "#ff86b8"
  sundae-pink-hover: "#ffa3c9"
  tote-orange: "#ff7a1f"
  hi-vis: "#f4b61a"
  exit-green: "#2fd37a"
  cold-store: "#6d98f0"
  meat-locker: "#f0606f"
typography:
  display:
    fontFamily: "General Sans, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(2rem, 0.9rem + 5.2vw, 5.25rem)"
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: "-0.03em"
  headline:
    fontFamily: "General Sans, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(2.125rem, 1.3rem + 3.4vw, 4.75rem)"
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: "-0.03em"
  title:
    fontFamily: "General Sans, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(1.25rem, 1.1rem + 0.7vw, 1.625rem)"
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: "-0.02em"
  body:
    fontFamily: "General Sans, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(1.0625rem, 1rem + 0.25vw, 1.1875rem)"
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: "General Sans, Segoe UI, system-ui, sans-serif"
    fontSize: "1rem"
    fontWeight: 500
    lineHeight: 1.1
  wordmark:
    fontFamily: "Bungee, Arial Black, Impact, sans-serif"
    fontSize: "1.375rem"
    fontWeight: 400
    lineHeight: 1
    letterSpacing: "0.02em"
rounded:
  none: "0"
  hole: "50%"
spacing:
  gutter: "clamp(16px, 4vw, 48px)"
  gap-sm: "8px"
  gap-md: "12px"
  gap-lg: "22px"
  band: "clamp(80px, 12vw, 180px)"
components:
  button-primary:
    backgroundColor: "{colors.sundae-pink}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "0 28px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.sundae-pink-hover}"
  button-ink:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.paper}"
    rounded: "{rounded.none}"
    padding: "0 28px"
    height: "56px"
  nav-button:
    backgroundColor: "{colors.sundae-pink}"
    textColor: "{colors.ink}"
    padding: "0 20px"
    height: "44px"
  paint-chip-card:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
    width: "1080px"
  swatch:
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "10px 12px"
    height: "64px"
  readout:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.paper}"
    padding: "20px 24px"
  slip:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    padding: "40px 32px 56px"
  label-strip-tile:
    textColor: "{colors.ink}"
    padding: "16px"
  reply-card:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    padding: "clamp(24px, 4vw, 48px)"
  download-stub:
    backgroundColor: "{colors.sundae-pink}"
    textColor: "{colors.ink}"
    height: "48px"
    padding: "0 20px 0 16px"
---

# Design System: Sundae Club

## Overview

**Creative North Star: "The Paint Fan Deck"**

The page is a hardware-shop paint card. The game is about matching paint to walls, so every section is a flat field of one real game colour, with a paint name where a label would go. Chapters change the page's colour: night violet for the hero and quiet sections, then Tote Orange, Cold Store blue, Hi-Vis, Sundae Pink, each as the whole background of its section. Content sits on paper-stock cards (the hero chip card, the slip, the reply card, the footer panel) laid over those fields.

Everything is flat and square. There are no gradients, no shadows, no rules and no rounded corners; the only curves are the punched-hole dots, the scalloped footer edge and the SVG suit. Depth comes from one flat card on another flat field, and from a few small rotations (crew fan, reply card). The only dark photographic surface is the dimmed hero video behind the chip card.

The voice is dry and loud: big tight General Sans headlines, one Bungee wordmark, one pink action colour. Humour lives in the copy, not the graphics.

**Key Characteristics:**
- Whole-section colour fields drawn from the game's own paint names
- Cool paper cards with ink text; night violet as the dark ground
- One action colour (Sundae Pink), one button shape (square, flat)
- Square corners everywhere; circles only as punched holes
- General Sans for all text, Bungee for the wordmark only

## Colors

A night-violet ground, cool paper cards, and six saturated paint colours that are the game's actual wall and suit colours.

### Primary
- **Sundae Pink** (#ff86b8): The one action colour: the Download button, the stub, wordmark, focus ring, text selection, and the Crew section field. Hover lightens to #ffa3c9.

### Secondary
- **Tote Orange** (#ff7a1f): Paint-section default wall, swatch and chip.
- **Hi-Vis** (#f4b61a): The Sponsors section field; a tile strip; a crew tag.
- **Exit Green** (#2fd37a): Swatch, tile strip, one place band, crew tag.
- **Cold Store** (#6d98f0): The Plan section field; swatch, chip, crew tag.
- **Meat Locker** (#f0606f): The Rookie's tag, one tile strip, a swatch.

### Neutral
- **Night** (#17142a): Nav, hero ground, Monsters and Download and footer grounds; also the ink colour on paper.
- **Night 2** (#211d38): The monsters aside note tile, a half-step off Night.
- **Paper** (#e8eaf0): Cool pale slate card stock for every card and the Places section.
- **Ink 2** (#413b58): Secondary text on paper (about 8:1).
- **Paper Dim** (#cfc9dc): Secondary text on Night (about 10:1).

### Named Rules
**The Real Paint Rule.** Fields and chips use only the six game colours above, each under its in-game name. Do not invent a seventh hue for decoration.
**The Ink On Colour Rule.** Text on any paint field or strip is Ink (#17142a), never white; light text appears only on Night and on Ink readouts.
**The One Pink Rule.** Pink is the action. Other fields may be pink (Crew) but buttons and the stub are always pink on a non-pink field, and Ink on the Download card.

## Typography

**Display Font:** General Sans (Fontshare, 400/500/700; fallback Segoe UI, system-ui)
**Body Font:** General Sans
**Wordmark Font:** Bungee, used for the nav wordmark only

**Character:** One grotesque used hard: tight, heavy, balanced headlines against plain 400 body. Bungee appears once, as the logo, and is not a display face for the page.

### Hierarchy
- **Display** (700, clamp 2rem to 5.25rem, 0.95, -0.03em): The hero h1 only, held to about 11 characters per line.
- **Headline** (700, clamp 2.125rem to 4.75rem, 0.95, -0.03em): Section h2s, held to 10 to 13ch.
- **Title** (700, clamp 1.25rem to 1.625rem, 1.1, -0.02em): Lead sentences (regular weight in leads), slip headings, tile, place and card names.
- **Body** (400, clamp 1.0625rem to 1.1875rem, 1.5): Paragraphs, kept to about 30 to 40ch in cards.
- **Label** (500, 1rem, 1.1): Swatch names, chip names, tile descriptors, tags, facts. Sentence case, no tracking.

### Named Rules
**The Balanced Headline Rule.** Headlines use text-wrap balance and a max-width in ch so they break like paint-card names.
**The One Logo Rule.** Bungee is the wordmark. Never set a heading, button or label in it.

## Layout

A 1360px wrap with a fluid gutter (16px to 48px). Sections are bands with generous vertical padding (80px to 180px). Intros use a 12-column grid (headline and lead in columns 1-6 or 1-7, a card in 7-12 or 8-12); the monsters are a 4-up tile grid; the crew is a 5-up fan. Gaps are 8px inside swatch pickers, 12px between tiles, 16 to 24px between columns.

The nav is a plain sticky Night bar (64px). The hero fills the first viewport with a centred chip card (max 800px) with five stacked colour chips left and copy right. A pink stub follows the scroll after the hero and hides at the Download section.

Responsive: below 900px two-column sections stack; below 720px the chip stack becomes a horizontal five-colour strip with names hidden; tiles go 4 to 2 to 1 columns; the crew fan flattens to 2 columns with no rotation; section nav links hide below 860px leaving the Download button.

## Elevation & Depth

Flat. There are no box-shadows anywhere. Layering is tonal and physical: a Paper card on a colour field, a Night section against a Paper one. Depth cues are limited to a card's small rotation (reply card 2deg, crew cards -6 to 6deg), the reply card overlapping into the footer (negative bottom margin), and a selected swatch lifting 6px.

### Named Rules
**The Flat Card Rule.** Never add shadows, gradients, blur or hairline rules to separate things. Separate with a change of flat fill.

## Shapes

Square corners (0 radius) on every card, button, swatch, tile and strip. The recurring silhouettes are: the punched hole (a 12 to 16px Night circle on the hero chips, stub and selected swatch), the torn slip edge (a clip-path sawtooth along the bottom of the job slip), and the scalloped footer edge (semicircle bumps in Paper above the back-of-card panel). Photos are cropped square, 16:10 or 3:4 and are never rounded.

## Components

### Buttons
- **Shape:** Square (0 radius), 56px tall, 28px side padding.
- **Primary:** Sundae Pink fill, Ink bold text. Nav version is 44px tall.
- **Ink variant:** Ink fill, Paper text, full width, used on the Paper reply card where pink would sit on a pink-adjacent field.
- **Hover / Focus:** Hover (pointer devices only) lightens pink to #ffa3c9; active presses to scale 0.97 in 160ms. Focus ring is a 3px Pink outline with 3px offset, Ink on paper surfaces.
- **Text link:** Weight 500, underlined, sits beside the button.

### Paint chip card (hero)
Paper card, no radius, 34/66 split: five stacked colour chips (names bottom-left in the label style, one Night punched hole at top-left) and the copy block. The h1, one lead, a facts line in Ink 2, one button and one link.

### Swatch picker
Six square swatch buttons in a 3-column grid, each filled with a game colour and named. Radio semantics with arrow-key navigation. Selected lifts 6px and shows an Ink dot top-right. An Ink readout block beneath shows the match percentage and verdict. The section background itself becomes the chosen wall colour (420ms fade).

### Job slip
Paper card with a sawtooth torn bottom edge, tabular numerals, title headings, items as bold lines with dot leaders to a right-aligned place, and an Ink total bar bleeding to the card edges.

### Label-strip tile
Square photo over a flat colour strip carrying a descriptor, a name and a sentence, all Ink. Strip colours cycle through the game palette (and Paper); one Night 2 note tile closes the grid.

### Place card
Night card with a 16:10 photo, light text, and a coloured name band (Cold Store or Exit Green) at the foot.

### Crew card (fan)
Paper cards with 3:4 portrait, name, and a palette-colour tag strip, rotated -6 to 6 degrees around the bottom, lifting 14px on hover.

### Reply card (download)
A Paper card rotated 2deg that overlaps the footer, with a headline, a full-width Ink button, file name, and a definition list of version, system, players and install.

### Download stub (bottom-right, hidden on phones and inside the paint demo)
Fixed bottom-left pink block with a Night punched hole and the label "Free playtest"; fades up after the hero, hides at Download.

### Footer
Scalloped Paper edge over a Paper "back of card" panel with a headline, links, a small stamped portrait in the corner and a centred imprint.

### Motion
Sections rise 24px and fade once (560ms, ease cubic-bezier(0.23, 1, 0.32, 1), 70ms stagger). Reduced motion removes the rise and the transitions, and pauses videos.

## Do's and Don'ts

### Do:
- **Do** colour a whole section with one game paint (#ff7a1f, #6d98f0, #f4b61a, #ff86b8) and put Paper cards on it.
- **Do** set text on paint fields and strips in Ink (#17142a).
- **Do** keep every corner square and every fill flat.
- **Do** give every swatch, chip or strip its in-game paint name.
- **Do** keep General Sans for all text and Bungee for the wordmark alone.
- **Do** keep touch targets at 44px or more and honour reduced motion.

### Don't:
- **Don't** add shadows, gradients, rounded corners or divider rules.
- **Don't** return to the old dark trailer-hero plus feature-card template or the camcorder/HUD chrome.
- **Don't** use any colour outside the thirteen tokens above.
- **Don't** put copy over photographs; copy sits on Paper, Night or a paint field.
- **Don't** add more than one pink action per view.
