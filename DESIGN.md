---
name: Synthetic Depth
colors:
  surface: '#0b1326'
  surface-dim: '#0b1326'
  surface-bright: '#31394d'
  surface-container-lowest: '#060e20'
  surface-container-low: '#131b2e'
  surface-container: '#171f33'
  surface-container-high: '#222a3d'
  surface-container-highest: '#2d3449'
  on-surface: '#dae2fd'
  on-surface-variant: '#b9cacb'
  inverse-surface: '#dae2fd'
  inverse-on-surface: '#283044'
  outline: '#849495'
  outline-variant: '#3a494b'
  surface-tint: '#00dbe7'
  primary: '#e1fdff'
  on-primary: '#00363a'
  primary-container: '#00f2ff'
  on-primary-container: '#006a71'
  inverse-primary: '#00696f'
  secondary: '#ecb2ff'
  on-secondary: '#520071'
  secondary-container: '#cf5cff'
  on-secondary-container: '#480063'
  tertiary: '#f9f6ff'
  on-tertiary: '#2f303b'
  tertiary-container: '#dad9e9'
  on-tertiary-container: '#5e5e6c'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#74f5ff'
  primary-fixed-dim: '#00dbe7'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#f8d8ff'
  secondary-fixed-dim: '#ecb2ff'
  on-secondary-fixed: '#320047'
  on-secondary-fixed-variant: '#74009f'
  tertiary-fixed: '#e2e1f1'
  tertiary-fixed-dim: '#c6c5d4'
  on-tertiary-fixed: '#1a1b26'
  on-tertiary-fixed-variant: '#454652'
  background: '#0b1326'
  on-background: '#dae2fd'
  surface-variant: '#2d3449'
typography:
  display:
    fontFamily: Geist
    fontSize: 64px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Geist
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-code:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.5'
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.1em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1280px
  gutter: 24px
  margin-mobile: 20px
  margin-desktop: 64px
---

## Brand & Style

This design system establishes a high-fidelity, futuristic environment for a full-stack developer portfolio. It merges the ethereal transparency of Glassmorphism with the tactile, physical presence of Neomorphism. The target audience includes technical recruiters and fellow developers who value precision, modern aesthetics, and sophisticated front-end execution.

The UI evokes a sense of "digital craftsmanship"—where elements feel like physical hardware interfaces embedded within a luminous, deep-space environment. The style prioritizes depth through layered transparency and soft, extruded geometry to create an interface that feels both cutting-edge and highly interactive.

## Colors

The palette is anchored in a deep, multi-tonal dark environment. The background is not a flat color but a gradient transition from Deep Navy (#0F172A) to a muted Charcoal/Purple (#1A1B26). 

Neon accents are used sparingly to highlight interactive states and critical information. 
- **Cyan (#00F2FF):** Represents "Active" states, code-related elements, and primary actions.
- **Violet (#BD00FF):** Used for "Feature" highlights, decorative gradients, and secondary visual interest.

Surface colors are derived from the neutral base with varying levels of opacity to facilitate the glass effect.

## Typography

The typography strategy emphasizes technical clarity and modern structure. 

**Geist** is utilized for headings to provide a sharp, geometric, and developer-centric feel. Its high x-height and tight tracking lend a premium, architectural quality to the portfolio.

**Inter** handles body copy, ensuring maximum readability across various screen densities. Its neutral tone balances the high-impact display type.

**JetBrains Mono** is reserved for metadata, labels, and code snippets, reinforcing the developer narrative through its distinct monospaced character.

## Layout & Spacing

This design system employs a fluid 12-column grid for desktop, transitioning to a 4-column grid for mobile. The spacing rhythm is strictly based on an 8px baseline to maintain mathematical harmony between the "soft" neomorphic elements and "sharp" technical content.

Section padding is generous to allow the background gradients and glass blurs to breathe. Content is primarily housed within centered containers, with occasional "bleeding" decorative elements to enhance the sense of depth.

## Elevation & Depth

Depth is achieved through a specific hierarchy of effects:

1.  **Background Layer:** Deep Navy to Purple gradient with a subtle noise texture to prevent banding.
2.  **Neomorphic Base:** Subtle extrusions built using dual shadows. For "raised" elements, use a light shadow (-4px, -4px, 12px) at 5% white opacity and a dark shadow (4px, 4px, 12px) at 40% black opacity.
3.  **Glass Panels:** Placed atop neomorphic bases. Use a `backdrop-filter: blur(12px)` with a background color of `rgba(255, 255, 255, 0.03)`.
4.  **The "Tech-Border":** All glass panels must feature a 1px solid border at 10% white opacity to define the edges against the dark background.
5.  **Interactive Glow:** On hover, primary elements emit a soft Cyan or Violet outer glow (spread 20px) to simulate light emission.

## Shapes

The shape language is "Soft-Modern." Surfaces use a consistent 0.5rem (8px) corner radius to bridge the gap between the organic feel of Neomorphism and the structured nature of code editors.

- **Buttons/Cards:** 16px (`rounded-lg`) to provide a friendly, tactile touchpoint.
- **Form Inputs:** 8px (`rounded-md`) for a more disciplined, technical appearance.
- **Status Indicators:** Fully circular (pill-shaped) to represent "active" light sources.

## Components

### Buttons
- **Primary:** Neomorphic "pressed" state on active. Uses a Cyan glow text shadow and a subtle 1px border.
- **Secondary:** Transparent glass with a 1px Violet border.

### Tactile Cards
Project cards should use the "raised" neomorphic base with a glass top-layer. On hover, the card should transition to a "pressed" state (inner shadow) to simulate physical feedback.

### Glowing Indicators
Use small 8px circles with a `box-shadow` of the same color (Cyan for "available for work") to create a breathing light effect.

### Frosted Forms
Inputs use a "sunken" neomorphic effect (inner shadows) with a high backdrop-filter blur. The cursor and focus border should utilize the Cyan accent.

### Code Blocks
Rendered on a deep #050505 background with 50% opacity, featuring the signature 1px border and JetBrains Mono typography.