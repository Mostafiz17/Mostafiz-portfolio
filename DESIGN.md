---
name: Obsidian Glass
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#c1c6d7'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#8b90a0'
  outline-variant: '#414755'
  surface-tint: '#adc6ff'
  primary: '#adc6ff'
  on-primary: '#002e69'
  primary-container: '#4b8eff'
  on-primary-container: '#00285c'
  inverse-primary: '#005bc1'
  secondary: '#e9b3ff'
  on-secondary: '#510074'
  secondary-container: '#7d01b1'
  on-secondary-container: '#e5a9ff'
  tertiary: '#ffb595'
  on-tertiary: '#571e00'
  tertiary-container: '#ef6719'
  on-tertiary-container: '#4c1a00'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc6ff'
  on-primary-fixed: '#001a41'
  on-primary-fixed-variant: '#004493'
  secondary-fixed: '#f6d9ff'
  secondary-fixed-dim: '#e9b3ff'
  on-secondary-fixed: '#310048'
  on-secondary-fixed-variant: '#7200a3'
  tertiary-fixed: '#ffdbcc'
  tertiary-fixed-dim: '#ffb595'
  on-tertiary-fixed: '#351000'
  on-tertiary-fixed-variant: '#7c2e00'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-2xl:
    fontFamily: Outfit
    fontSize: 72px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  display-lg:
    fontFamily: Outfit
    fontSize: 48px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Outfit
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.3'
  headline-md-mobile:
    fontFamily: Outfit
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  container-max: 1200px
  gutter: 24px
  margin-desktop: 64px
  margin-mobile: 20px
  section-gap: 128px
---

## Brand & Style

This design system is engineered for high-end digital portfolios and creative showcases, blending the precision of developer tools with the cinematic elegance of luxury hardware brands. The personality is **technically precise** yet **emotionally resonant**, evoking the feeling of a futuristic cockpit or a high-performance studio.

The visual style is a sophisticated evolution of **Glassmorphism**, termed "Obsidian Glass." It utilizes deep, multi-layered dark surfaces, high-fidelity backdrop blurs, and hyper-thin "light-leak" strokes. Contrast is managed through luminance rather than pure color, using soft neon accents to guide the eye toward primary actions and critical data points. The overall aesthetic should feel expensive, calm, and effortlessly modern.

## Colors

The palette is anchored in **Deep Obsidian (#0A0A0A)**, providing a high-contrast foundation for light and color to play. 

- **Primary (Electric Blue):** Used for primary actions, focus states, and active indicators. It represents precision.
- **Secondary (Cyber Purple):** Used for creative highlights, secondary actions, and decorative gradients. It represents imagination.
- **Surface Strategy:** Instead of solid grays, surfaces use varying opacities of white over the obsidian base, combined with `backdrop-filter: blur(20px)`.
- **Neon Accents:** Subtle "glow" effects are achieved through low-opacity box shadows and radial gradients rather than solid fills, ensuring the UI feels luminous rather than heavy.

## Typography

The typography strategy balances bold, geometric expression with utilitarian clarity.

- **Headlines:** Use **Outfit** (a contemporary alternative to Poppins with better screen rendering) for a bold, cinematic presence. Tracking should be tightened on larger sizes to create a "locked-in" editorial look.
- **Body:** **Inter** handles all long-form content, providing exceptional legibility on dark backgrounds. 
- **Metadata:** **JetBrains Mono** is introduced for labels, tags, and technical specs, reinforcing the "technically precise" personality of the system.
- **Hierarchy:** Use generous vertical rhythm. Titles should feel like "hero" moments, while body text remains unobtrusive.

## Layout & Spacing

The layout philosophy is rooted in **Generous Whitespace** and a **Fluid Fixed Grid**. Content is centered within a 1200px container for optimal readability, but background elements (like glass panels and gradients) should bleed to the edges of the viewport.

- **The 8px Rule:** All spacing increments follow a strict 4px/8px grid to maintain mathematical harmony.
- **Negative Space:** Use massive gaps (128px+) between major sections to allow the "Obsidian" background to act as a visual reset.
- **Mobile Adaptation:** On mobile, margins shrink to 20px, and section gaps reduce to 64px. Multi-column grids (3 or 4 columns) must collapse into a single vertical stack.

## Elevation & Depth

Depth is not created with traditional shadows, but through **Luminance and Translucency**.

1.  **Level 0 (Base):** Pure Obsidian (#0A0A0A).
2.  **Level 1 (Card/Surface):** Semi-transparent glass (`rgba(255,255,255, 0.03)`) with a 1px border (`rgba(255,255,255, 0.08)`) and a 20px backdrop blur.
3.  **Level 2 (Hover/Active):** Increase glass opacity to 0.06 and add a subtle primary-colored glow (`0 8px 32px rgba(0, 122, 255, 0.1)`).
4.  **Level 3 (Modals/Popovers):** Highest contrast glass with a secondary "rim light" stroke on the top edge to simulate physical depth.

Shadows should be "Ambient" — extremely diffused (40px-80px blur) and tinted with the primary or secondary neon colors to create a soft atmospheric glow.

## Shapes

The shape language is **Softly Geometric**. 

A radius of **0.5rem (8px)** is the standard for cards and inputs, providing a modern, refined look that feels friendlier than sharp corners but more professional than pill shapes. 

- **Small Components:** Buttons and chips use a slightly more aggressive **1rem** radius to make them feel tactile and "clickable."
- **Outer Containers:** Large layout sections or main wrappers should use **1.5rem (24px)** when nested within the viewport to create a "device-within-a-device" aesthetic.

## Components

### Buttons
- **Primary:** Solid Electric Blue background with white text. Apply a subtle outer glow of the same color.
- **Secondary (Glass):** Blurred glass background with a thin 1px white border (10% opacity). Text in white.
- **Interaction:** On hover, primary buttons should increase their glow intensity; secondary buttons should increase their backdrop-filter strength.

### Cards
- Cards must use the Level 1 Elevation (Backdrop blur + 1px border). 
- Content inside cards should have a 32px internal padding.
- Images inside cards should have a subtle 1px inner overlay to prevent them from looking "flat" against the glass.

### Inputs & Form Fields
- Backgrounds are dark and recessed. 
- The bottom border or the entire stroke glows Electric Blue only when the field is focused.
- Labels use JetBrains Mono in a muted gray color.

### Chips & Tags
- Tiny, capsule-shaped elements.
- Use Cyber Purple for "Creative" or "Design" tags and Electric Blue for "Technical" or "Code" tags.
- Backgrounds should be highly transparent (5-10% opacity) with high-contrast text.

### Scroll Progress Indicator
- A thin, 2px neon gradient line (Blue to Purple) at the very top of the viewport to indicate reading progress.