---
name: CrewCase
description: Gear tracking for film and video crews
colors:
  orange: "#E8822A"
  orange-dim: "rgba(232,130,42,0.13)"
  blue: "#3A7BD5"
  blue-dim: "rgba(58,123,213,0.13)"
  green: "#30D158"
  green-dim: "rgba(48,209,88,0.16)"
  red: "#FF453A"
  red-dim: "rgba(255,69,58,0.13)"
  purple: "#BF5AF2"
  purple-dim: "rgba(191,90,242,0.16)"
  bg-void: "#08080b"
  bg-raised: "#111115"
  surface: "#17171c"
  surface-high: "#202026"
  border-subtle: "rgba(255,255,255,0.07)"
  border-visible: "rgba(255,255,255,0.12)"
  ink: "#f5f5f7"
  ink-muted: "rgba(245,245,247,0.5)"
  ink-faint: "rgba(245,245,247,0.25)"
  light-bg: "#f2f2f7"
  light-ink: "#1c1c1e"
  light-ink-muted: "rgba(28,28,30,0.5)"
typography:
  display:
    fontFamily: "Inter, -apple-system, BlinkMacSystemFont, SF Pro Display, sans-serif"
    fontSize: "clamp(42px, 7.5vw, 78px)"
    fontWeight: 900
    lineHeight: 1.04
    letterSpacing: "-2.5px"
  headline:
    fontFamily: "Inter, -apple-system, BlinkMacSystemFont, SF Pro Display, sans-serif"
    fontSize: "clamp(28px, 4.5vw, 44px)"
    fontWeight: 800
    lineHeight: 1.1
    letterSpacing: "-1.5px"
  title:
    fontFamily: "Inter, -apple-system, BlinkMacSystemFont, SF Pro Display, sans-serif"
    fontSize: "16px"
    fontWeight: 700
    lineHeight: 1.4
    letterSpacing: "normal"
  body:
    fontFamily: "Inter, -apple-system, BlinkMacSystemFont, SF Pro Display, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
    letterSpacing: "normal"
  label:
    fontFamily: "Inter, -apple-system, BlinkMacSystemFont, SF Pro Display, sans-serif"
    fontSize: "11px"
    fontWeight: 700
    lineHeight: 1.4
    letterSpacing: "2px"
  mono:
    fontFamily: "JetBrains Mono, monospace"
    fontSize: "13px"
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: "normal"
rounded:
  pill: "50px"
  card: "18px"
  badge: "14px"
  step: "10px"
  logo: "8px"
  bar: "2px"
spacing:
  xs: "6px"
  sm: "14px"
  md: "26px"
  lg: "52px"
  xl: "88px"
  section-max: "1080px"
components:
  button-primary:
    backgroundColor: "{colors.orange}"
    textColor: "#ffffff"
    rounded: "{rounded.pill}"
    padding: "15px 30px"
  button-primary-hover:
    backgroundColor: "{colors.orange}"
    textColor: "#ffffff"
    rounded: "{rounded.pill}"
    padding: "15px 30px"
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.ink-muted}"
    rounded: "{rounded.pill}"
    padding: "14px 26px"
  button-nav:
    backgroundColor: "{colors.orange}"
    textColor: "#ffffff"
    rounded: "{rounded.pill}"
    padding: "9px 20px"
  pill-green:
    backgroundColor: "{colors.green-dim}"
    textColor: "{colors.green}"
    rounded: "{rounded.pill}"
    padding: "3px 10px"
  pill-orange:
    backgroundColor: "{colors.orange-dim}"
    textColor: "{colors.orange}"
    rounded: "{rounded.pill}"
    padding: "3px 10px"
  pill-red:
    backgroundColor: "{colors.red-dim}"
    textColor: "{colors.red}"
    rounded: "{rounded.pill}"
    padding: "3px 10px"
  pill-purple:
    backgroundColor: "{colors.purple-dim}"
    textColor: "{colors.purple}"
    rounded: "{rounded.pill}"
    padding: "3px 10px"
  card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.card}"
    padding: "26px"
  input:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "14px 18px"
---

# Design System: CrewCase

## 1. Overview

**Creative North Star: "The Camera Report"**

A camera report is the daily log that a film crew fills out to account for every roll, every mag, every piece of equipment that touched the camera. It is precise, complete, and non-negotiable. That is the sensibility of this design system: every element earns its place on the page the same way every line earns its place on a report. No decoration for decoration's sake. No color that doesn't carry information.

The system is built for the dark — deep near-black backgrounds that mirror the color temperature of a set, with one warm accent (film orange) that signals action. Status information is carried by a tight, iOS-native color vocabulary (green/orange/red/purple) that crews already know from their phones. Typography is heavy and compressed at display sizes, then relaxes into readable Inter for body copy. The experience should feel like picking up an industry tool you've never used before and immediately understanding it.

This system explicitly rejects: generic SaaS productivity aesthetics (Notion-style light neutrals, airy whitespace), consumer lifestyle softness (rounded corners on everything, pastel tints, playful microcopy), and enterprise coldness (rigid grids, corporate blues, technical jargon as copy). It also rejects the current wave of "film brand" cliches: grain overlays without purpose, fake film stock filters, serif-on-black as a shorthand for "cinematic."

**Key Characteristics:**
- Deep dark background with near-zero lightness (#08080b) — not charcoal, not slate, void
- Single warm accent (orange #E8822A) carried sparingly; its rarity is the signal
- Status expressed entirely through a four-color semantic vocabulary, never through shape alone
- Typography compressed hard at display sizes; Inter at maximum weight (-2.5px tracking at 900)
- Surfaces layer in discrete steps: bg-void → bg-raised → surface → surface-high
- Motion is functional — scroll reveals and hover lifts only; no choreography for its own sake

## 2. Colors

A near-void dark field with one warm signal color and a four-status semantic vocabulary inherited from iOS.

### Primary
- **Cine Orange** (`#E8822A`): The brand's single voice. Used on CTAs, active states, the logo mark, the promo bar, and the hero gradient. Never used decoratively. When this color appears, it means "act" or "this matters."
- **Orange Tint** (`rgba(232,130,42,0.13)`): The surface variant of Cine Orange. Used as background for chips, eyebrows, and the "OUT" status pill. Pairs with Cine Orange as text.

### Secondary
- **Gear Blue** (`#3A7BD5`): Reserved for stats callouts and secondary accent contexts. Never used on CTAs. Conveys information, not urgency.
- **Blue Tint** (`rgba(58,123,213,0.13)`): Surface variant. Rarely used; present in the token set for future status contexts.

### Tertiary
- **Signal Green** (`#30D158`): iOS-native green. The "IN" status — gear is available. Also used for success states (form confirmation).
- **Green Tint** (`rgba(48,209,88,0.16)`): Surface for the IN pill and success banners.
- **Alert Red** (`#FF453A`): iOS-native red. The "OVERDUE" status and error states. High urgency.
- **Red Tint** (`rgba(255,69,58,0.13)`): Surface for the OVERDUE pill.
- **Maint Purple** (`#BF5AF2`): iOS-native purple. The "MAINT" status — gear is out of service. Lower urgency than red.
- **Purple Tint** (`rgba(191,90,242,0.16)`): Surface for the MAINT pill.

### Neutral
- **Void** (`#08080b`): The primary page background. Not charcoal. Not navy. Near-black with a faint warm undertone that keeps it from reading as pure digital black.
- **Raised** (`#111115`): The secondary page background used for alternating sections (screens band, testimonials, showcase). Creates section rhythm without borders.
- **Surface** (`#17171c`): Card backgrounds, navigation, footer. The primary interactive surface layer.
- **Surface High** (`#202026`): Elevated surfaces for nested containers or future modals.
- **Border Subtle** (`rgba(255,255,255,0.07)`): Default borders on cards and surface dividers. Barely perceptible — structural, not decorative.
- **Border Visible** (`rgba(255,255,255,0.12)`): Active input borders, button outlines, hover-state borders.
- **Ink** (`#f5f5f7`): Primary text. Apple's standard near-white for dark UI; slightly warm, never harsh.
- **Ink Muted** (`rgba(245,245,247,0.5)`): Secondary/supporting text. Navigation links, body copy on dark backgrounds, labels.
- **Ink Faint** (`rgba(245,245,247,0.25)`): Decorative text. Phone screen labels, trusted-by section names. Do not use for any text that needs to be read.
- **Light BG** (`#f2f2f7`): Apple systemGray6 — used for the features grid section as a light-mode break. Provides contrast against the surrounding dark sections.
- **Light Ink** (`#1c1c1e`): Apple systemGray1 — primary text on the light section.
- **Light Ink Muted** (`rgba(28,28,30,0.5)`): Secondary text on light sections.

### Named Rules
**The One Voice Rule.** Cine Orange appears on ≤2 interactive elements visible at any time (promo bar, primary CTA, or active state). When it appears everywhere, it means nothing. Its presence is the signal; dilute it and the signal is lost.

**The Status Contract.** Green = available, Orange = checked out, Red = overdue, Purple = maintenance. These four roles are fixed and non-negotiable. Do not use these colors outside their status context — no "green for success in a generic sense," no "red for a sale." Film crews read these as instrument readouts, not decorative choices.

## 3. Typography

**Display / Body Font:** Inter (with -apple-system, BlinkMacSystemFont, SF Pro Display fallback)
**Mono Font:** JetBrains Mono 500

**Character:** Inter pushed to its extremes — weight 900 with -2.5px tracking at display sizes collapses the letterforms into a dense, editorial block. Then the same family relaxes to 400 weight and 1.7 line-height for body copy. The contrast between the two modes is what gives the page energy. JetBrains Mono appears sparingly for technical labels and code-adjacent UI.

### Hierarchy
- **Display** (900, clamp(42px–78px), line-height 1.04, -2.5px tracking): Hero headline only. Maximum compression. The `em` color accent (Cine Orange on a key word) is the only inline color treatment permitted in display type.
- **Headline** (800, clamp(28px–44px), line-height 1.1, -1.5px tracking): Section headings (`h2`). Tight but not as compressed as display. Used for split sections, waitlist CTA.
- **Title** (700–800, 16px, line-height 1.4): Card titles, step titles, feature titles. Body-scale headings that rely on weight rather than size for hierarchy.
- **Body** (400–500, 16–17px, line-height 1.7, max 65ch): Section subheadings, feature descriptions, split-section copy. Cap line length at 65–75ch. `var(--muted)` on dark, `var(--light-ink-muted)` on light.
- **Label** (700, 11px, letter-spacing 2px, uppercase): Section eyebrows, phone screen labels, trusted-by section identifier. Used sparingly — maximum 1 visible per section. Never as a substitute for a real heading.
- **Mono** (JetBrains Mono 500, 13px): Available for technical callouts. Not in use on the current landing page; present for future app-adjacent UI.

### Named Rules
**The Compression Rule.** Display type must be at weight 900 and letter-spacing ≤ -2px. Dropping to 700 or removing negative tracking at display sizes makes the page feel like a template. The compressed block is the brand's typographic identity.

**The Eyebrow Budget.** One uppercase tracked label (`sect-eyebrow`) per section maximum. Never stack two eyebrows. If a section needs a label, use the eyebrow or the title — not both plus a subheading badge.

## 4. Elevation

The system uses tonal layering, not shadows, as the primary depth mechanism. Dark sections alternate between bg-void (#08080b) and bg-raised (#111115) to create rhythm without visible borders between sections. Card surfaces (surface, #17171c) sit visually above both backgrounds simply by being lighter.

Shadows exist in two specific contexts only: the iPhone device frame (structural, high-drama), and the primary CTA button glow (functional signal). No cards or containers have drop shadows in the dark theme. The light section uses a single soft box-shadow on cards.

### Shadow Vocabulary
- **Device Frame** (`0 0 0 1.5px rgba(255,255,255,0.13), 0 0 0 3px #000, 0 48px 96px rgba(0,0,0,0.8), 0 16px 40px rgba(0,0,0,0.55)`): iPhone mockup frames only. The double-ring highlight simulates the physical phone edge. Never apply this shadow to UI elements.
- **CTA Glow** (`0 6px 28px rgba(232,130,42,0.35)`): Primary button only. The warm glow anchors the CTA in the page and reinforces the orange brand color without adding a new visual element.
- **Light Card** (`0 2px 14px rgba(0,0,0,0.07)`): Cards in the light-background features section only. Soft and ambient. No dark-theme equivalent.

### Named Rules
**The Flat-By-Default Rule.** Dark surfaces are flat at rest. Shadows exist only on the device frame (because it is a physical object) and the primary CTA (because it is the conversion point). Everything else earns depth through tonal layering. Adding box-shadows to cards or nav on dark backgrounds reads as web-circa-2016, not as a cinema tool.

## 5. Components

### Buttons
Pill-shaped across all variants. The shape is borrowed from iOS native controls — crews already associate this form with tappable UI.

- **Shape:** Fully rounded pill (50px radius on all button variants)
- **Primary:** Cine Orange background, white text, padding 15px 30px (desktop) / 14px 26px (nav variant), CTA Glow box-shadow. The only element with a persistent shadow in the dark theme.
- **Hover / Focus:** `opacity: 0.87` + `translateY(-2px)` at 0.2s ease. No color change on hover — dimming preserves the brand color.
- **Outline / Ghost:** Transparent background, ink-muted text, border-visible border. Hover shifts to ink text and border opacity 0.25. Paired with Primary in the hero CTA group as the secondary option.
- **Nav CTA:** Same as Primary at reduced padding (9px 20px) for the navigation context.

### Status Pills
The semantic vocabulary of the app, rendered on the landing page as a feature preview. Tight and badge-like.

- **Shape:** Pill (50px radius), padding 3px 10px, font 11px weight 700 uppercase
- **Four variants:** green (IN), orange (OUT), red (OVERDUE), purple (MAINT)
- **Rule:** Each pill uses the tinted background of its color against the full-saturation text. Never use a solid-color background on pills — the semi-transparent tint ensures legibility on both dark and light surfaces.

### Cards / Containers
- **Corner Style:** Gently rounded (18px radius) — softer than the pill shape but tighter than typical SaaS cards
- **Background:** `var(--surface)` (#17171c) on dark sections; `#ffffff` on the light features section
- **Shadow Strategy:** No shadow on dark cards (tonal layering only); soft ambient shadow on light cards (`0 2px 14px rgba(0,0,0,0.07)`)
- **Border:** `1px solid var(--border-subtle)` on dark cards; no border on light cards
- **Internal Padding:** 26px standard; 28px on testimonial cards
- **Hover:** `translateY(-3px)` at 0.2s for feature cards; no hover on testimonial cards

### Inputs / Fields
- **Style:** Pill shape (50px radius), `var(--surface)` background, `border-visible` border, 14px 18px padding
- **Focus:** Border shifts to Cine Orange (`var(--orange)`). No glow or box-shadow — the color change is the signal.
- **Placeholder:** `var(--ink-muted)` — meets 3:1 contrast on `var(--surface)` background
- **Submit button:** Inline within the email form row, same Primary button treatment

### Navigation
- **Style:** Fixed, `rgba(8,8,11,0.9)` background with `backdrop-filter: blur(24px)`, 1px `border-subtle` bottom border. Offset from top by 34px (height of promo bar).
- **Logo:** 32px orange rounded square (8px radius) + "CrewCase" in Inter 800, weight 800, -0.4px tracking
- **Links:** 14px Inter 500, ink-muted default, transitions to ink on hover at 0.2s
- **Mobile:** Nav links (`Features`, `How it works`) hide at 720px; CTA remains visible

### Device Frame (Signature Component)
The iPhone mockup is the most visually distinctive element on the page — it is the product. Every screen is presented inside a realistic device frame.

- **Shape:** 50px border-radius, black background, hidden overflow (clips screenshot)
- **Chrome detail:** Double-ring edge highlight (`0 0 0 1.5px rgba(255,255,255,0.13), 0 0 0 3px #000`) simulates physical phone edge
- **Dynamic Island:** Pseudo-element at top center — 32% width, 30px height, 20px radius, z-index 30
- **Shadow:** High-drama depth shadow (see Device Frame in Elevation)
- **Rule:** Never show app screenshots outside a device frame on the landing page. The frame is what communicates "this is a real iOS app," not a mockup.

### Section Eyebrow
A recurring micro-element: small uppercase tracked label above section headings.

- **Style:** 11px Inter 700, uppercase, 2px letter-spacing, `var(--orange)` color, 12px bottom margin
- **Budget:** One per section maximum. If the section doesn't need a label, omit it entirely rather than inventing one.

## 6. Do's and Don'ts

### Do:
- **Do** use `var(--orange)` (#E8822A) for CTAs, active states, and the logo mark. It is the single primary signal color.
- **Do** keep display type at weight 900, letter-spacing ≤ -2px. The compressed block is the typographic identity.
- **Do** use tonal layering (bg-void → bg-raised → surface) for depth on dark sections. No box-shadows on containers.
- **Do** use the four-status color vocabulary (green/orange/red/purple) strictly for gear status. These colors are semantic contracts, not decorative options.
- **Do** present every app screenshot inside an iPhone device frame. The frame communicates "this is a real, shipped iOS app."
- **Do** cap section eyebrows to one per section. If a section doesn't need a label, omit it.
- **Do** maintain `prefers-reduced-motion` support on all transitions and animations. The current implementation (0.01ms override) is the correct approach.
- **Do** use `var(--border-subtle)` (7% white) on dark card borders. Visible borders on dark surfaces look like web-2010 UI.

### Don't:
- **Don't** use a light or cream background as the page default. The dark void background is non-negotiable — this tool lives on dark sets, dark monitors, dark environments.
- **Don't** apply gradient text (`background-clip: text`). Use Cine Orange as a solid color on a key word in the hero headline; that's the only inline type treatment.
- **Don't** add box-shadows to dark-theme cards or containers. Tonal layering carries depth; shadows on dark surfaces look like a 2016 web template.
- **Don't** use Cine Orange on more than one or two elements visible simultaneously. Its rarity is the signal. If it appears on every section eyebrow, every icon bar, and every card accent, it becomes noise.
- **Don't** use the status colors (green, red, purple) outside their semantic status contexts. Alert Red is not a general-purpose error color. Signal Green is not a general-purpose success color.
- **Don't** design for generic SaaS aesthetics: no light neutrals as the page base, no airy whitespace sections in isolation, no Notion/Linear-style cards with large padding and minimal content.
- **Don't** design for consumer lifestyle softness: no pastel tints, no bubbly rounded-corner-everything, no playful or casual microcopy.
- **Don't** use numbered section markers (01 / 02 / 03) as eyebrows. The How It Works step numbers are legitimate (they are a real ordered sequence). Numbered eyebrows on every section are AI scaffolding.
- **Don't** use all-caps body copy. Uppercase is reserved for labels ≤ 4 words.
- **Don't** show app screenshots without a device frame. A raw screenshot floating on the background reads as a design tool mockup, not a shipped product.
