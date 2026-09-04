---
name: Vow & Vine
description: Event services from birthdays to weddings, Central Oregon — The Golden Hour Garden
colors:
  ivory: "#f7f3ec"
  ivory-2: "#fbf8f2"
  paper: "#ffffff"
  gold: "#b08d57"
  gold-soft: "#c5a877"
  sage: "#7c8767"
  sage-deep: "#5f6a4e"
  ink: "#2c2a26"
  taupe: "#6b6256"
  line: "#e6ddcd"
typography:
  display:
    fontFamily: "Cormorant Garamond, Georgia, serif"
    fontSize: "clamp(2.6rem, 6.4vw, 4.8rem)"
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: "0.08em"
  headline:
    fontFamily: "Cormorant Garamond, Georgia, serif"
    fontSize: "clamp(2rem, 4.4vw, 3rem)"
    fontWeight: 600
    lineHeight: 1.1
  title:
    fontFamily: "Cormorant Garamond, Georgia, serif"
    fontSize: "1.4rem"
    fontWeight: 600
    lineHeight: 1.2
  body:
    fontFamily: "Jost, system-ui, sans-serif"
    fontSize: "1rem"
    fontWeight: 300
    lineHeight: 1.75
  label:
    fontFamily: "Jost, system-ui, sans-serif"
    fontSize: "0.76rem"
    fontWeight: 400
    letterSpacing: "0.36em"
rounded:
  sm: "8px"
  md: "14px"
  lg: "22px"
  button: "2px"
spacing:
  sm: "16px"
  md: "26px"
  lg: "48px"
  section: "clamp(4rem, 8vw, 7rem)"
components:
  button-gold:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.paper}"
    rounded: "{rounded.button}"
    padding: "1rem 2rem"
  button-gold-hover:
    backgroundColor: "{colors.gold-soft}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.button}"
    padding: "1rem 2rem"
  card-service:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.md}"
    padding: "1.9rem 1.6rem"
---

# Design System: Vow & Vine

## Overview

**Creative North Star: "The Golden Hour Garden"**

Vow & Vine is a late-afternoon garden in the hour before the ceremony begins — ivory light, soft gold catching on a champagne flute, the first rustle of sage in a warm wind. The design system is botanical and airy: a cream-warm ivory ground that never feels harsh, gold that reads as warmth rather than flash, and sage-green as the unexpected botanical counterpoint. Nothing in this system competes with the emotion the visitor brings to the page.

Cormorant Garamond carries the editorial weight, set at generous uppercase tracking for the hero title — a bridal program, not a news headline. Body text is Jost at light weight (300), deliberately soft so the serif headings have clear authority. Pinyon Script appears as flourishes only: the hero monogram, the ampersand in the brand name, and one inline emphasis per page. SVG vine ornaments frame the hero with a stroke-drawing animation and pace the scroll.

The system is open and low-density. Section padding is generous. Service cards center their content. Nothing crowds. This is the breathing room before the first dance.

**Key Characteristics:**
- Ivory warm ground — never clinical white
- Sage as the botanical complement to gold — nature grounds the romance
- Cormorant Garamond uppercase at wide tracking — bridal program register
- Near-square buttons, delicate border — unhurried formality
- SVG vine path animation draws on load via stroke-dashoffset

## Colors

Ivory, champagne, sage — the palette of a garden wedding in soft afternoon light.

### Primary
- **Champagne Gold** (`#b08d57`): Buttons, eyebrow labels, border accents, icon hover state, vine ornament accents. Warm and earthy — more antique than flashy.
- **Soft Champagne** (`#c5a877`): Button hover state, footer heading labels. Slightly lighter and warmer.

### Secondary
- **Garden Sage** (`#7c8767`): Service card icons at rest, vine SVG paths, the partners ribbon background. Botanical counterweight to gold.
- **Deep Sage** (`#5f6a4e`): Sage icon hover state, eyebrow labels on the sage-background ribbon. The darker grounding tone.

### Neutral
- **Warm Ivory** (`#f7f3ec`): Page background. Slightly warm linen — not a screen's pure white.
- **Soft Ivory** (`#fbf8f2`): Section alternates, hero gradient, feature section background.
- **Paper** (`#ffffff`): Card surfaces, form fields. Pure white as contrast inside the ivory ground.
- **Deep Earth** (`#2c2a26`): Primary headings and h1 text. Near-black with brown warmth.
- **Taupe** (`#6b6256`): Lead paragraphs, card descriptors, nav links, footer links.
- **Warm Line** (`#e6ddcd`): All borders and dividers. Beige-warm rather than grey.

### Named Rules
**The Sage Accent Rule.** Sage holds the icons at rest and the decorative vines. Gold takes over on hover. Sage is the garden; gold is the light. Never both at full saturation simultaneously on the same element.

## Typography

**Display Font:** Cormorant Garamond (Georgia, serif)
**Body Font:** Jost weight 300 (system-ui fallback)
**Script Accent:** Pinyon Script — hero monogram, the `&` ampersand in the logotype, one inline `em` per hero

**Character:** Cormorant Garamond at uppercase with wide tracking reads like a formal invitation card. Jost at light weight (300) provides airy body copy that defers to the serifs. The Pinyon Script monogram at 4.4rem above the hero title sets the ceremonial opening.

### Hierarchy
- **Display** (500, clamp 2.6–4.8rem, lh 1.1, ls 0.08em, uppercase): Hero h1 brand name. Always paired with the Pinyon Script monogram above and the brand tagline in small-caps Jost below.
- **Headline** (600, clamp 2–3rem, lh 1.1): Section h2. Deep earth color; italic gold `em` span for one word of emphasis.
- **Title** (600, 1.4rem, lh 1.2): Service and event card h3. Cormorant Garamond; deep earth.
- **Body** (300, 1rem, lh 1.75): Jost light. Taupe. Max ~48ch per line for comfortable reading.
- **Label** (400, 0.76rem, ls 0.36em, uppercase): Eyebrow, nav links, button labels, footer headings. Gold by default.

### Named Rules
**The Light-Body Rule.** Jost body text is always weight 300. Never increase to 400 or 500 in the body — the lightness is the system's breathing room. Bold text in the body disrupts the airy pacing.

## Layout

Container max-width 1160px, 26px padding. Hero: centered single-column, max 800px content width, with SVG vines positioned absolutely at the left and right edges (hidden below 920px). Section padding: `clamp(4rem, 8vw, 7rem)`. Service and family grids: three-column (two at 920px, one at 600px). Feature/wedding split: 50/50 (stacks at 920px). Partners ribbon: centered flex row of pill-outline serif tags on sage-deep background. Scroll-reveal: 800ms ease, 26px translateY, 100ms stagger. Vine stroke animation: 3s ease, 0.2s delay, on page load.

Breakpoints: 920px (tablet — vines hidden, grids collapse), 600px (mobile — hamburger, single column).

## Elevation & Depth

Warm amber-tinted shadows at three scales. Shadows read as soft afternoon light rather than neutral grey. Cards rest flat without shadow; hover adds the Lifted shadow. The CTA block and form card carry the Lifted shadow at rest as their primary depth signal.

### Shadow Vocabulary
- **Whisper** (`0 2px 10px rgba(75,64,45,.06)`): Subtle hover presence on credential-style elements.
- **Lifted** (`0 18px 40px rgba(75,64,45,.10)`): Card hover, CTA block at rest, form card at rest.
- **Floating** (`0 30px 70px rgba(75,64,45,.14)`): Reserved for the single most prominent element per page view.

### Named Rules
**The Garden Depth Rule.** Shadows are warm amber, not grey. The shadow color is derived from the ink color (`rgba(75,64,45)`) so depth reads as earth and light, not concrete.

## Shapes

Near-square buttons (2px radius) — formal, like a sealed envelope corner. Cards use a gentle radius scale: 8px small, 14px medium, 22px large. Service card content is center-aligned, unlike the left-aligned patterns in the other brands — centering signals ceremony. The vine-divider ornament (sage SVG lines flanking a small gold leaf) appears between the hero and first section. No pill-shaped elements in this system.

## Components

### Buttons
- **Shape:** Near-square (2px radius), Jost 400, 0.8rem, ls 0.2em, uppercase
- **Gold Primary:** Champagne Gold (`#b08d57`) background, white text, 1rem×2rem padding
- **Hover:** Soft Champagne background, –2px translateY, gold shadow
- **Ghost:** Transparent, 1px warm-line border, ink text → sage border and sage-deep text on hover

### Cards / Containers
- **Service Card:** Paper white, 1px warm-line border, 14px radius, 1.9rem×1.6rem padding, center-aligned. Icon: 50px, sage → gold on hover.
- **Split Photo:** 460px height, 14px radius, 1px warm-line border.
- **CTA Block:** Paper white, 1px warm-line border, 22px radius, Lifted shadow at rest.
- **Partners Tags:** Pill-shaped (999px), 1px white-25% border on sage-deep background, Cormorant Garamond 1.15rem — the one pill shape in the entire system, on the sage ribbon only.

### Navigation
- **Style:** Frosted ivory glass (85% warm-ivory, 12px blur), 84px height, 1px warm-line bottom border
- **Links:** Jost 400, 0.8rem, ls 0.14em, uppercase, taupe → ink on hover; 1px gold underline from left
- **Logo:** Cormorant Garamond 1.3rem, deep earth, ls 0.14em; micro Jost gold label below
- **Mobile:** Hamburger at 600px; vine ornaments hidden at 920px

### Vine Divider (Signature Component)
Center-aligned flex row: 120px sage SVG vine path (left), 12px gold leaf diamond center, 120px sage SVG vine path (right, mirrored). Vine paths draw via stroke-dashoffset (900 → 0, 3s ease, 0.2s delay) on load. Appears immediately below the hero on every page. Used optionally between major alternating sections.

## Do's and Don'ts

### Do:
- **Do** keep the hero display title uppercase at 0.08em tracking — the bridal program register defines the brand.
- **Do** include the vine-divider ornament below every hero.
- **Do** center-align all service card content.
- **Do** animate vine SVG paths on page load — the stroke-drawing is the site's opening signature.
- **Do** let icons rest in sage and shift to gold on hover.

### Don't:
- **Don't** increase Jost body weight beyond 300 — the lightness is structural.
- **Don't** use colored backgrounds other than the sage-deep partners ribbon in any section.
- **Don't** use Pinyon Script in body text or headings. It appears only in the hero monogram, the `&` ampersand, and one inline emphasis span per hero.
- **Don't** add vine ornaments inside content sections — they are page-structural (hero/section top), not fill decorations.
- **Don't** apply shadow to resting cards. Shadow is reserved for hover and the CTA/form blocks.
