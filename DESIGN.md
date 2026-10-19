---
name: Jayson Williams Landscaping
description: Your yard. Our work. A spruce-green phone-first pitch site whose signature is a lawn the visitor mows.
colors:
  mower-orange: "#ef7d2d"
  mower-orange-hi: "#f79a52"
  orange-ink: "#1e1207"
  spruce: "#12302a"
  spruce-raised: "#1a3f37"
  dew: "#edf2e6"
  dew-shade: "#dbe5d1"
  ink: "#14261f"
  ink-soft: "#3d5649"
  on-dark: "#f1f5ec"
  on-dark-soft: "#bccdbd"
  grass: "#93c862"
  step-green: "#4a8434"
  chip-on: "#2a5a2b"
  turf: "#2f5722"
  stripe-light: "#6aa443"
  stripe-dark: "#41792d"
  mulch: "#3a2516"
  leaf-rust: "#d8612a"
  leaf-gold: "#e9a23b"
  focus-blue: "#5aa9ff"
  focus-blue-deep: "#1f6fd1"
  error-peach: "#ffb08a"
  placeholder: "#9db3a2"
  field-line: "rgba(241,245,236,.5)"
  hairline-ink: "rgba(20,38,31,.14)"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(40px, 13.6vw, 6rem)"
    fontWeight: 900
    lineHeight: 0.92
    letterSpacing: "-0.02em"
  display-slogan:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(28px, 8.2vw, 5.2rem)"
    fontWeight: 900
    lineHeight: 0.94
    letterSpacing: "-0.03em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(1.9rem, 8vw, 3rem)"
    fontWeight: 900
    lineHeight: 0.98
    letterSpacing: "-0.02em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "20px"
    fontWeight: 800
    lineHeight: 1.2
  lead:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 20px)"
    fontWeight: 400
    lineHeight: 1.45
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 800
    lineHeight: 1.1
  small:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.55
rounded:
  tick: "5px"
  control: "12px"
  button: "14px"
  lawn-panel: "18px"
  round: "50%"
spacing:
  gap: "10px"
  field: "18px"
  gutter: "20px"
  gutter-wide: "32px"
  section: "60px"
  column-gap: "80px"
components:
  button-primary:
    backgroundColor: "{colors.mower-orange}"
    textColor: "{colors.orange-ink}"
    typography: "{typography.label}"
    rounded: "{rounded.button}"
    padding: "0 16px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.mower-orange-hi}"
    textColor: "{colors.orange-ink}"
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.label}"
    rounded: "{rounded.button}"
    padding: "0 16px"
    height: "56px"
  input-field:
    backgroundColor: "{colors.spruce-raised}"
    textColor: "{colors.on-dark}"
    typography: "{typography.body}"
    rounded: "{rounded.control}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.spruce-raised}"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.control}"
    padding: "6px 12px"
    height: "52px"
  chip-checked:
    backgroundColor: "{colors.chip-on}"
    textColor: "{colors.on-dark}"
  service-row:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.title}"
    padding: "10px 2px"
    height: "60px"
  service-arrow:
    backgroundColor: "{colors.dew-shade}"
    textColor: "{colors.ink}"
    rounded: "{rounded.round}"
    size: "38px"
  service-arrow-hover:
    backgroundColor: "{colors.mower-orange}"
    textColor: "{colors.orange-ink}"
---

# Design System: Jayson Williams Landscaping

## Overview

**Creative North Star: "The Fresh-Cut Lawn"**

The site is a yard on a fall afternoon: deep spruce ground, a dew-light working section, and a living lawn that a small orange push mower cuts into light and dark stripes while autumn leaves drift onto it. The visitor can take the handle and mow it. Every other surface is plain and strong, like a crew's truck lettering: heavy uppercase display, sentence-case body, one orange for every action.

Density is phone-first and generous: one column at 360 to 430px, big touch targets (52 to 60px), short copy. On desktop the hero splits into copy and lawn side by side, and the services and steps sit in two columns. Depth comes from the lawn's own material (stripes, mulch, leaves, clippings, the mower's cast shadow), never from UI chrome.

Confirmed rejections from the direction: the landscaper template's stock lawn photo, icon-card services grid, and stat counters. Under Ellie's pitch-site house rules: no web font, no sticky bottom bar, no black page ground.

**Key Characteristics:**
- Spruce-and-dew grounds; mower orange is the only action color and the mower itself.
- Heavy uppercase system sans for display and wordmark; plain sentence-case body.
- The mowable lawn is the signature, repeated as hero lawn, grass divider strip, desktop side lawn, and closing lawn.
- Flat UI; the only shadow belongs to the mower on the grass.
- Blue outlines mean "this control is live" on form controls and focus.

## Colors

A two-ground green system (spruce dark, dew light) with a single hot orange and a lawn palette that lives inside the canvas.

### Primary
- **Mower Orange** (`mower-orange`): every action fill (Get a free quote, Text us this request), the service arrow on hover/focus, and the mower's deck. Text on it is always Orange Ink.
- **Mower Orange High** (`mower-orange-hi`): hover state of orange fills, and hover color for the header phone link and footer links.
- **Orange Ink** (`orange-ink`): text and icons sitting on orange.

### Secondary
- **Fresh Grass** (`grass`): the phone icon, the "Landscaping" line of the wordmark, checked-chip border and tick, and text selection. A light accent for dark ground only.
- **Step Green** (`step-green`): the large step numerals on the dew section.
- **Chip-On Green** (`chip-on`): checked chip fill.

### Tertiary (lawn material, canvas and fallback only)
- **Stripe Light / Stripe Dark** (`stripe-light`, `stripe-dark`): the cut-grass stripe pair; also the no-JS repeating stripe fallback under each canvas (44px bands).
- **Turf** (`turf`): shaggy uncut grass base and the divider strip's background.
- **Mulch** (`mulch`): the bed edge along the hero lawn (top edge on phones, left edge on desktop).
- **Leaf Rust / Leaf Gold** (`leaf-rust`, `leaf-gold`): falling leaves and the leaf-bit spray when Leaf removal is ticked.

### Neutral
- **Spruce** (`spruce`): page ground, header, hero, quote, close, footer. Also the theme-color.
- **Spruce Raised** (`spruce-raised`): input and chip fill on spruce.
- **Dew** (`dew`): the services-and-steps working section.
- **Dew Shade** (`dew-shade`): resting service-arrow disc.
- **Ink / Ink Soft** (`ink`, `ink-soft`): text on dew; Ink Soft for step descriptions and the "homes and businesses" line.
- **On-Dark / On-Dark Soft** (`on-dark`, `on-dark-soft`): text on spruce; Soft for the promise line, area line, notes, footer copy.
- **Field Line** (`field-line`): 2px input and chip border on spruce.
- **Ink Hairline** (`hairline-ink`): the 1px rules between service rows.
- **Focus Blue / Focus Blue Deep** (`focus-blue`, `focus-blue-deep`): outlines only. Deep is used where the ring sits on dew.
- **Error Peach** (`error-peach`): field error text and invalid-field border on spruce.

### Named Rules
**The Mower Orange Rule.** Orange is the action color and the mower, nothing else. No orange headings, borders, rules, or decoration. Leaves are rust and gold, not mower orange.

**The Two Grounds Rule.** Every section sits on Spruce or Dew. No black ground, no third surface color; the lawn is the only other "ground".

**The Blue Means Live Rule.** Focus Blue appears only as an outline: on form controls and the submit button at hover and focus, and as the global focus-visible ring. Use Focus Blue Deep where the ring lands on Dew.

## Typography

**Display Font:** system sans stack (-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif) at weight 900, uppercase
**Body Font:** the same stack at 400

**Character:** One family doing two jobs: a shouted, tightly tracked uppercase for the slogan and section heads, and plain conversational sentence case for everything a homeowner reads. The system stack is a sanctioned house-rule decision (no web font; no client logo exists, so the wordmark is set in this lettering).

### Hierarchy
- **Display** (900, clamp 40px to 6rem; desktop clamp 4rem to 6.4rem; phone held sideways clamp 2.4rem to 3.4rem; line-height 0.92, -0.02em, uppercase): the hero headline only, two lines that each stay on one line ("Your yard." / "Our work.").
- **Display Slogan** (900, clamp 28px to 5.2rem; desktop clamp 3rem to 4.4rem; 0.94, -0.03em, uppercase): the closing three-line slogan above the closing lawn.
- **Headline** (900, clamp 1.9rem to 3rem, 0.98, -0.02em, uppercase): section heads (What we do, Getting a quote, Get a free quote.).
- **Title** (800, 20px, 1.2): service row names; step titles at 800 19px/1.25.
- **Lead** (400, clamp 17px to 20px, desktop 22px, 1.45, max 30 to 31ch): the hero promise line.
- **Body** (400, 17px, 1.55): all running copy.
- **Label** (800, 17px): buttons, legends, field labels.
- **Small** (400 or 700, 16px): form note, error text, chip text.
- **Step numeral** (900, 34px, line-height 1, Step Green): the counter beside each step.
- **Wordmark** (900, 16px, desktop 18px, uppercase, +0.01em) over "Landscaping" (800, 11px, +0.3em, uppercase, Fresh Grass). A lockup, not a label style.

### Named Rules
**The Shout And Talk Rule.** Uppercase 900 is for display, headlines, the wordmark, and the footer name. Everything else is sentence case at 400 to 800. Never uppercase body, buttons, or labels.

**The Unbroken Line Rule.** Display lines are authored as separate spans that never wrap internally; the headline breaks at the slogan's own periods, not wherever the viewport cuts.

**The Display Carries Hierarchy Rule.** Body steps stay within 16 to 22px; the jump to the 40 to 96px display and 30 to 48px headline does the ranking. (Recorded as a detector exception for flat-type-hierarchy.)

## Layout

Phone-first single column with a 20px gutter (32px from 600px). Content width caps at 1180px. Section rhythm is 56 to 64px vertical padding (services 56/64, quote 60/64, close 60/0). Gaps are 10px between paired buttons and chips, 18px between fields, 22px between steps.

The first screen is header (wordmark left, phone number top-right), headline, promise, a two-button row (fill at 1.4fr, outline at 1fr, max 460px), and the hero lawn under them (clamp 280px to 460px tall, 44svh).

Breakpoints: 600px (gutter grows, chips flow inline instead of a two-column grid, hero lawn grows); phone landscape under 500px tall (hero splits copy and lawn side by side); 1024px desktop (hero becomes a 1.08fr / 1fr grid with the lawn filling the right column at min 560px; services and steps sit 1.1fr / 1fr with an 88px gap; quote becomes 1fr / 1.3fr with an 80px gap and the side lawn fills the space under the quote heading). Desktop header and hero copy align their left edge to the 1180px content column.

**The Lawn Interval Rule.** The lawn is the section divider: hero lawn after the first screen, a 30px grass strip between the dew section and the quote, a side lawn beside the form on desktop only, and the closing lawn under the slogan. New sections are separated by lawn or by a ground change, never by drawn rules or cards.

## Elevation & Depth

The UI is flat: no box-shadows on any button, field, chip, row, or panel. Depth is conveyed by ground change (spruce vs dew vs lawn) and by the lawn's own material: shaggy tufts over cut stripes, a mulch edge with an inner darkening gradient, leaves with radial shading, and the mower's soft cast shadow on the grass (blur 5px, rgba(6,18,4,.5), offset 2.5px / 4.5px).

### Named Rules
**The Only Shadow Is On The Grass Rule.** Shadows exist only inside the lawn canvas, cast by objects on it. Interface elements never cast shadows.

## Shapes

Softly rounded rectangles for everything touchable: 14px on buttons, 12px on fields and chips, 5px on the chip tick box, 18px on the desktop side lawn panel. The service arrow is the one circle (38px disc). Service rows are square, ruled by 1px Ink Hairlines top and bottom of the list and between rows (a ruled list, recorded as a detector exception). Full-bleed lawns (hero, strip, close) have no radius; the side lawn is the only clipped, rounded lawn. Borders are 2px on controls, 1px on rules.

## Components

### Buttons
Confident, thumb-sized, and few.
- **Shape:** gently rounded (`rounded.button`), 56px min height, 2px border.
- **Primary (fill):** Mower Orange fill and border, Orange Ink text, Label type. Hover (hover-capable devices only) shifts to Mower Orange High. Active nudges down 1px.
- **Outline:** transparent, On-Dark text, border On-Dark at 55%; hover brightens the border to full On-Dark with an 8% On-Dark wash. Used only as the secondary hero action (Text us).
- **In the form:** the submit button is full width and gains the Focus Blue outline (2px, offset 3px) on hover and focus, matching the other form controls.
- **Transitions:** 0.18s on color properties, 0.12s transform; all removed under reduced motion.

### Chips (service checkboxes)
- **Style:** Spruce Raised fill, 2px Field Line border, 52px min height, 12px radius, 16px/700 text, with a drawn 18px tick box (5px radius) before the label. Two-column grid on phones, inline wrap from 600px.
- **Checked:** Chip-On Green fill, Fresh Grass border, tick box filled Fresh Grass with an Ink check.
- **Hover / Focus:** 2px Focus Blue outline, 2px offset.
- **Behavior:** ticking one plays a 260ms scale pop and sprays 8 grass clippings (leaf bits for Leaf removal); skipped under reduced motion.

### Inputs / Fields
- **Style:** Spruce Raised fill, 2px Field Line border, 12px radius, 13px/14px padding, 52px min height (textarea 96px, vertical resize), 17px text, orange caret, Placeholder color for hints.
- **Hover / Focus:** 2px Focus Blue outline, 2px offset; the border itself does not change.
- **Error:** border turns Error Peach and a 16px/700 Error Peach message appears below. Labels are 800 17px above the field; "(optional)" sits in 400 On-Dark Soft.

### Navigation (header)
- **Style:** a single bar, 64px min height, no background change and not sticky. Wordmark left (links to top), phone number right with a Fresh Grass phone icon, 800 16px (18px desktop), tabular numerals.
- **Hover:** phone link text goes Mower Orange High. No other nav.

### Service Rows
- **Style:** full-width ruled rows on Dew, 60px min height, Title type in Ink, a 38px Dew Shade arrow disc at the right.
- **Hover / Focus:** only the arrow changes: disc goes Mower Orange with Orange Ink arrow, arrow slides 2px right. Keyboard focus adds a 3px Focus Blue Deep ring on the disc. The row itself never tints, outlines, or shadows.
- **Behavior:** tapping a row ticks that service in the form, scrolls to the quote, and pops the chip.

### Living Lawn (signature)
A canvas lawn of shaggy fall grass (4 tuft greens over a Turf base) that a push mower cuts into alternating light/dark stripes. Cut grass holds, then regrows over about 9 seconds. The mower autopilots in boustrophedon rows and hands control to the visitor's pointer or thumb, resuming after 2.5s idle. Leaves fall and are mulched into a spray of rust and gold bits; grass clippings spray from the deck. Tunables live in the engine's CFG block (cell 3px, deck 50px phone up to 64px, tuft gap and length 11px, wind 3.2px, 14 leaves, 28 on wide lawns).
- **Instances:** hero (mower, leaves, mulch edge), close (mower, leaves), side (desktop only, mower, leaves, 18px radius), strip (30px tall, grass only, parts under the pointer, 4 leaves).
- **Fallback:** a 44px repeating Stripe Light / Stripe Dark gradient sits under every canvas (detector exception).
- **Motion and input:** pauses off-screen; under reduced motion the lawn renders one pre-mowed still frame, touch scrolls the page, and the cursor returns.

## Do's and Don'ts

### Do:
- **Do** put every action on Mower Orange with Orange Ink text, and keep the mower the same orange.
- **Do** set display and section heads in 900 uppercase system sans with -0.02em to -0.03em tracking, and keep each display line on one line.
- **Do** separate sections with lawn or a Spruce/Dew ground change.
- **Do** give form controls (inputs, textarea, chips, submit) a Focus Blue (#5aa9ff) outline on hover and focus.
- **Do** gate every hover style behind `(hover:hover)`.
- **Do** keep touch targets at 52px or more (buttons 56px, service rows 60px).
- **Do** show the phone number on the first screen only in the header's top-right, and the email only in the footer.
- **Do** honor reduced motion: still lawn, no pops, no transitions.

### Don't:
- **Don't** use a stock lawn photo, an icon-card services grid, or stat counters.
- **Don't** load a web font or replace the wordmark with an invented logo.
- **Don't** add a sticky bottom bar.
- **Don't** tint, outline, or shadow a service row on hover; only its arrow changes, from neutral to orange.
- **Don't** use orange for anything that is not an action or the mower.
- **Don't** put box-shadows on interface elements.
- **Don't** use a black page ground.
- **Don't** add small tracked uppercase labels or eyebrows above headings; the tracked "Landscaping" line belongs to the wordmark only.
