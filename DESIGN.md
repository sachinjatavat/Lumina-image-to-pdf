---
name: Lumina Convert
colors:
  surface: '#f7f9fb'
  surface-dim: '#d8dadc'
  surface-bright: '#f7f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#eceef0'
  surface-container-high: '#e6e8ea'
  surface-container-highest: '#e0e3e5'
  on-surface: '#191c1e'
  on-surface-variant: '#464555'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#777587'
  outline-variant: '#c7c4d8'
  surface-tint: '#4d44e3'
  primary: '#3525cd'
  on-primary: '#ffffff'
  primary-container: '#4f46e5'
  on-primary-container: '#dad7ff'
  inverse-primary: '#c3c0ff'
  secondary: '#565e74'
  on-secondary: '#ffffff'
  secondary-container: '#dae2fd'
  on-secondary-container: '#5c647a'
  tertiary: '#7e3000'
  on-tertiary: '#ffffff'
  tertiary-container: '#a44100'
  on-tertiary-container: '#ffd2be'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2dfff'
  primary-fixed-dim: '#c3c0ff'
  on-primary-fixed: '#0f0069'
  on-primary-fixed-variant: '#3323cc'
  secondary-fixed: '#dae2fd'
  secondary-fixed-dim: '#bec6e0'
  on-secondary-fixed: '#131b2e'
  on-secondary-fixed-variant: '#3f465c'
  tertiary-fixed: '#ffdbcc'
  tertiary-fixed-dim: '#ffb695'
  on-tertiary-fixed: '#351000'
  on-tertiary-fixed-variant: '#7b2f00'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  display-lg:
    fontFamily: Geist
    fontSize: 72px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  display-lg-mobile:
    fontFamily: Geist
    fontSize: 40px
    fontWeight: '800'
    lineHeight: '1.2'
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: Geist
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.03em
  headline-md:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.3'
    letterSpacing: -0.02em
  body-lg:
    fontFamily: Geist
    fontSize: 20px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: -0.01em
  body-md:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  label-md:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: 0.05em
  mono-label:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.2'
    letterSpacing: 0.1em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  container-max: 1280px
  gutter: 32px
  margin-mobile: 20px
  margin-desktop: 64px
  stack-sm: 8px
  stack-md: 24px
  stack-lg: 64px
  section-gap: 128px
---

## Brand & Style

The design system is centered on a **Premium Minimalist** aesthetic, tailored for a high-end utility tool that feels more like a creative studio than a functional script. It targets professional creators, legal executives, and designers who value speed, privacy, and aesthetic clarity.

The UI evokes an emotional response of **composed confidence**. By utilizing a "Luminous" foundation, the design system avoids the cluttered anxiety of traditional file converters. It leans heavily into an **airy, editorial layout** with sophisticated glassmorphism and subtle tactile feedback. The primary objective is to make the act of file conversion feel like a premium experience rather than a digital chore.

## Colors

The palette is intentionally restrained to maintain an atmosphere of high-end sophistication.

- **Luminous White (#FFFFFF/F8FAFC):** Used for large surface areas and background layers to create an expansive, airy feel.
- **Midnight Slate (#0F172A):** This serves as the primary ink for typography and structural icons, providing a grounded, authoritative contrast.
- **Serene Indigo (#4F46E5):** A precision accent color used sparingly for primary actions, progress indicators, and focus states. 

Avoid using standard "success" green or "error" red unless absolutely necessary for accessibility; instead, use tonal shifts of Indigo or Slate to communicate state changes.

## Typography

This design system uses **Geist** exclusively to maintain a technical yet refined personality. The type scale is built on an editorial model with aggressive "tight" kerning for large headings.

- **Headlines:** Use Bold or ExtraBold weights. Negative letter-spacing is mandatory for Display and Headline roles to achieve the high-end "stamped" look.
- **Body Text:** Use Regular weight with generous line height (1.6) to ensure the layout remains breathable and legible.
- **Labels:** Small labels and tags should use a slightly heavier weight and increased letter-spacing to provide a functional contrast to the fluid body text.

## Layout & Spacing

The layout philosophy follows a **Fixed-Fluid hybrid grid**. Content is contained within a max-width of 1280px, centered on the screen, but background elements and glass containers may bleed to the edges.

- **Vertical Rhythm:** Use a generous 128px gap between major landing page sections to reinforce the "airy" brand promise. 
- **The 8px Rule:** All internal component spacing must be a multiple of 8px.
- **Mobile Adaption:** On mobile devices, margins shrink to 20px, and section gaps should be halved. Complex multi-column grids must reflow into a single-column stack with center-aligned typography for headers.

## Elevation & Depth

This design system uses a combination of **Tonal Layering** and **Glassmorphism** to establish hierarchy.

1.  **Base Layer:** Luminous White or very light Slate (#F8FAFC).
2.  **Surface Layer:** Pure White cards with 1px semi-transparent Slate borders (5% opacity).
3.  **Floating Elements:** Use extremely soft, large-radius shadows. 
    *   *Shadow Specs:* `0 20px 50px rgba(15, 23, 42, 0.05)`.
4.  **Glass Containers:** For file upload zones and navigation bars, use a backdrop-blur of 12px with a white tint at 70% opacity. This creates a "frosted" look that keeps the UI feeling modern and lightweight.

## Shapes

The shape language is sophisticated and approachable. All primary containers use a **12px (0.75rem)** radius.

- **Buttons & Inputs:** Follow the standard 12px radius.
- **Large Cards/Glass Sections:** Use `rounded-xl` (1.5rem / 24px) to create a soft, welcoming frame for primary content.
- **Interactive Elements:** On hover, shapes should not change radius, but rather increase in shadow depth or surface brightness to indicate state.

## Components

### Buttons
- **Primary:** Solid Midnight Slate with white text. High-contrast, sharp, and authoritative.
- **Secondary:** Transparent background with 1px Midnight Slate border.
- **Tertiary:** Pure text with an underline that appears on hover, utilizing Serene Indigo.

### Drop Zone / File Upload
This is the "hero" component. It should feature a large glassmorphic container with a dashed 2px border in light Indigo. The background should have a subtle gradient from white to #F8FAFC.

### Input Fields
Minimalist styling. No background fill—only a bottom border of 1px in light Slate. On focus, the border transitions to Serene Indigo with a subtle 4px outer glow.

### Chips & Tags
Used for file formats (e.g., .JPG, .PNG). Small, pill-shaped, using a light Indigo tint background (#E0E7FF) and Midnight Slate text.

### Progress Bars
Ultra-thin (4px height). The track is light Slate, and the indicator is a solid Serene Indigo line with a soft glow effect at the leading edge.

### Navigation
A "sticky" top bar with a glassmorphic background blur. Icons should be stroke-based (1.5px weight) in Midnight Slate.