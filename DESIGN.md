---
name: Cinematic Creative
colors:
  surface: '#121414'
  surface-dim: '#121414'
  surface-bright: '#37393a'
  surface-container-lowest: '#0c0f0f'
  surface-container-low: '#1a1c1c'
  surface-container: '#1e2020'
  surface-container-high: '#282a2b'
  surface-container-highest: '#333535'
  on-surface: '#e2e2e2'
  on-surface-variant: '#e4bfb1'
  inverse-surface: '#e2e2e2'
  inverse-on-surface: '#2f3131'
  outline: '#ab897d'
  outline-variant: '#5b4137'
  surface-tint: '#ffb599'
  primary: '#ffb599'
  on-primary: '#5a1c00'
  primary-container: '#ff5e00'
  on-primary-container: '#531900'
  inverse-primary: '#a63b00'
  secondary: '#ffb599'
  on-secondary: '#5a1c00'
  secondary-container: '#802f07'
  on-secondary-container: '#ffa17b'
  tertiary: '#9fcaff'
  on-tertiary: '#003258'
  tertiary-container: '#0097fb'
  on-tertiary-container: '#002d51'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdbce'
  primary-fixed-dim: '#ffb599'
  on-primary-fixed: '#370e00'
  on-primary-fixed-variant: '#7f2b00'
  secondary-fixed: '#ffdbce'
  secondary-fixed-dim: '#ffb599'
  on-secondary-fixed: '#370e00'
  on-secondary-fixed-variant: '#7d2d04'
  tertiary-fixed: '#d1e4ff'
  tertiary-fixed-dim: '#9fcaff'
  on-tertiary-fixed: '#001d36'
  on-tertiary-fixed-variant: '#00497d'
  background: '#121414'
  on-background: '#e2e2e2'
  surface-variant: '#333535'
typography:
  display-hero:
    fontFamily: Inter
    fontSize: 72px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.05em
  display-hero-mobile:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.05em
  headline-md:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  metadata-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: 0.4em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  container-max: 1440px
  gutter: 24px
  margin-mobile: 20px
  margin-desktop: 80px
  transition-timing: cubic-bezier(0.4, 0, 0.2, 1)
---

## Brand & Style
This design system is built for high-end creative agencies and production houses. It leverages a **Cinematic Glassmorphism** style—blending deep, obsidian backgrounds with high-contrast accents and ethereal translucent layers. The aesthetic is designed to feel like a premium viewing experience, prioritizing high-impact imagery and smooth motion. The emotional response is one of sophistication, innovation, and "behind-the-scenes" exclusivity.

Key visual pillars include:
- **Depth through Transparency:** Layers of frosted glass create a sense of physical space.
- **High-Impact Contrast:** Extreme typographic scale paired with vibrant hits of color against a dark void.
- **Precision Motion:** Every interaction follows a specific cubic-bezier curve to mimic the ease-of-use of high-end camera gear or professional editing suites.

## Colors
The palette is centered on a "Midnight Studio" theme. The primary background is a near-absolute black to ensure visual depth. The accent color, a vibrant Flare Orange, is used sparingly for calls to action and active states to guide the eye without overwhelming the content.

White is used exclusively in varying opacities to establish hierarchy:
- **High Emphasis (100%):** Headlines and primary actions.
- **Medium Emphasis (60%):** Body text and active icons.
- **Low Emphasis (40%):** Metadata, taglines, and secondary labels.
- **Subtle (10% - 20%):** Borders, dividers, and inactive states.

## Typography
The typographic system relies on extreme variance in scale and tracking. 

- **Headlines:** Use `ExtraBold` weights with negative letter-spacing for a "tight," impactful feel. Hero headers should dominate the viewport.
- **Body:** Prioritize readability with a generous line height (1.6) and reduced opacity to keep the focus on visual assets.
- **Metadata/Taglines:** These use wide-tracked uppercase styles to provide a technical, "data-stamped" appearance similar to film slates or technical blueprints.

## Layout & Spacing
The layout follows a fluid-grid philosophy with generous margins to create an "editorial" feel. 

- **Desktop:** A 12-column grid with 80px side margins to allow the content to breathe.
- **Mobile:** A 4-column grid with 20px margins.
- **Vertical Rhythm:** Use large vertical spacing (120px - 160px) between major sections to emphasize the "Cinematic" pace, allowing each piece of content to be viewed in isolation.
- **Motion:** All layout transitions must use the `cubic-bezier(0.4, 0, 0.2, 1)` timing function for a smooth, high-end feel.

## Elevation & Depth
Elevation is not achieved through traditional shadows, but through **translucency and blur**. 

- **Surface 1 (Base):** The #0a0a0a background.
- **Surface 2 (Glass):** Used for cards and navigation. Background of `rgba(255, 255, 255, 0.05)`, a 1px solid border of `rgba(255, 255, 255, 0.1)`, and a `backdrop-filter: blur(12px)`.
- **Active Elevation:** When an element is hovered or focused, it may emit a soft glow using a primary-tinted shadow (e.g., `32px` blur, `rgba(255, 94, 0, 0.1)`).

## Shapes
The design system uses a **Rounded** (0.5rem base) language for standard components like cards and inputs to feel approachable. However, for specialized interactive elements like navigation bars and scroll indicators, a **Pill-shaped** (rounded-full) approach is used to differentiate "Tools" from "Content."

## Components

### Navigation Bar
A fixed, floating bar at the top or bottom of the screen.
- **Style:** `rounded-full`, `backdrop-filter: blur(12px)`, background `rgba(255, 255, 255, 0.1)`.
- **Border:** 1px solid `rgba(255, 255, 255, 0.1)`.

### Glassmorphism Buttons
- **Base:** Glass surface with white text.
- **Hover State:** Background shifts to `rgba(255, 94, 0, 0.2)`, border changes to `rgba(255, 94, 0, 0.4)`, and a 32px glow shadow of `rgba(255, 94, 0, 0.1)` is applied.
- **Transition:** Smooth cubic-bezier on all properties.

### Scroll Indicator
- **Style:** A floating 40x40px circle.
- **Border:** 1px solid `rgba(255, 255, 255, 0.2)`.
- **Animation:** Subtle vertical "bounce" or "pulse" to indicate interactivity.

### Cards
- **Background:** `rgba(255, 255, 255, 0.05)`.
- **Blur:** 12px backdrop blur.
- **Padding:** 32px (Desktop), 24px (Mobile).

### Input Fields
- **Style:** Underlined or subtle glass backgrounds with 40% opacity placeholder text.
- **Focus:** Border transitions to the Primary Accent color with a subtle outer glow.