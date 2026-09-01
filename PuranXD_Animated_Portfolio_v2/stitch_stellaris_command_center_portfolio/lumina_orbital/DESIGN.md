---
name: Lumina Orbital
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
  on-surface-variant: '#c4c7c8'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#8e9192'
  outline-variant: '#444748'
  surface-tint: '#c6c6c7'
  primary: '#ffffff'
  on-primary: '#2f3131'
  primary-container: '#e2e2e2'
  on-primary-container: '#636565'
  inverse-primary: '#5d5f5f'
  secondary: '#adc6ff'
  on-secondary: '#002e6a'
  secondary-container: '#0566d9'
  on-secondary-container: '#e6ecff'
  tertiary: '#ffffff'
  on-tertiary: '#00363e'
  tertiary-container: '#a0efff'
  on-tertiary-container: '#006f7d'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e2e2e2'
  primary-fixed-dim: '#c6c6c7'
  on-primary-fixed: '#1a1c1c'
  on-primary-fixed-variant: '#454747'
  secondary-fixed: '#d8e2ff'
  secondary-fixed-dim: '#adc6ff'
  on-secondary-fixed: '#001a42'
  on-secondary-fixed-variant: '#004395'
  tertiary-fixed: '#a0efff'
  tertiary-fixed-dim: '#5dd6ec'
  on-tertiary-fixed: '#001f25'
  on-tertiary-fixed-variant: '#004e59'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
  surface-glass: rgba(15, 23, 42, 0.45)
  border-ethereal: rgba(255, 255, 255, 0.08)
  accent-purple: '#9B82FF'
  glow-blue: rgba(59, 130, 246, 0.15)
typography:
  display-xl:
    fontFamily: Inter
    fontSize: 72px
    fontWeight: '700'
    lineHeight: 80px
    letterSpacing: -0.04em
  display-xl-mobile:
    fontFamily: Inter
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '500'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.1em
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.2em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 24px
  margin-mobile: 20px
  margin-desktop: 80px
  container-max: 1440px
---

## Brand & Style

The design system embodies the persona of a **Digital Architect**—someone who builds structures in the infinite void of the web. The brand personality is "Futuristic Precision," blending the hyper-clean aesthetic of high-end hardware with the immersive atmosphere of a space command center.

The visual style is a fusion of **Minimalism** and **Glassmorphism**. It relies on deep blacks to create a sense of infinite depth, while UI elements appear as "projected" glass interfaces floating in space. Every interaction should feel cinematic, utilizing low-opacity glows and razor-thin borders to define structure without adding visual bulk.

**Key visual principles:**
- **Vastness:** Use generous white space (the "void") to make content feel significant.
- **Luminance:** Color is used sparingly as light, not just decoration.
- **Precision:** Monospaced accents provide a technical, "data-driven" layer to the sophisticated sans-serif foundation.

## Colors

The palette is anchored by **Deep Black (#050505)** to ensure perfect contrast and true-black depth on OLED screens. 

- **Primary White:** Used for high-priority typography and core structural icons.
- **Soft Blue Glow:** Acts as the primary "energy" color, used for active states, primary buttons, and ambient light leaks.
- **Surface Glass:** A dark navy translucent layer that creates the illusion of depth through backdrop blurring.
- **Ethereal Borders:** Extremely low-opacity white lines that define edges without breaking the fluid visual flow of the background.

## Typography

The typographic hierarchy balances bold, aggressive headlines with hyper-readable technical labels. 

**Inter** is the workhorse, providing a clean, Swiss-inspired clarity. For the "Command Center" feel, use **JetBrains Mono** for secondary data points, code snippets, and metadata labels. 

- **Display Text:** Use negative letter-spacing for large headlines to create a tight, architectural feel.
- **Labels:** Always use uppercase or monospaced styling for labels to distinguish them as "system readouts" rather than narrative text.
- **Responsive Scaling:** On mobile, reduce display sizes significantly to prevent horizontal scrolling, focusing on vertical hierarchy.

## Layout & Spacing

This design system uses a **Fluid Grid** with wide margins to evoke the emptiness of space. 

- **Grid Model:** 12-column grid for desktop with 24px gutters. Elements should often "float" across columns rather than being strictly boxed, especially for decorative orbits.
- **Cinematic Padding:** Section vertical padding should be aggressive (e.g., 160px+) to allow elements to breathe and feel like separate "stations" in a journey.
- **Alignment:** Use center-alignment for high-impact hero sections and left-alignment for technical or content-heavy blocks. 
- **Mobile:** Transition to a single-column layout with 20px side margins, maintaining the monospaced labels to keep the technical identity intact.

## Elevation & Depth

Depth is not communicated through shadows, but through **Tonal Layering and Blur**.

- **Level 0 (Background):** Pure #050505. May contain subtle animated particle fields (stars).
- **Level 1 (Glass Panes):** `surface-glass` with a `backdrop-filter: blur(12px)`. This creates a frosted "cockpit" feel.
- **Level 2 (Active Overlays):** Higher opacity glass or subtle `secondary-color` outer glows (e.g., `box-shadow: 0 0 30px rgba(59, 130, 246, 0.2)`).
- **Outlines:** Every elevated card or panel must have a 1px border using `border-ethereal`. This simulates the thin structural lines found in blueprints or HUDs.

## Shapes

The shape language is a mix of **Rounded Rectangles** and **Perfect Circles**.

- **Cards/Panels:** Use a consistent 0.5rem (8px) radius for a modern, balanced look.
- **Navigation/CTAs:** Utilize **Pill-shapes** (fully rounded) for navigation bars and buttons to create a "capsule" aesthetic.
- **Orbits:** Decorative elements should be perfect circles with thin, dashed borders to simulate orbital paths or radar sweeps.

## Components

### Buttons
- **Primary:** Pill-shaped, White background, black text. Subtle `secondary-color` glow on hover.
- **Ghost:** Pill-shaped, `border-ethereal` with white text. Fills with `surface-glass` on hover.

### Floating Navigation
- A centered, pill-shaped bar using `surface-glass`. 
- Active links should be signaled by a small circular "node" underneath the text or a subtle blue text glow.

### Cards & Panels
- Use `surface-glass` with a 1px `border-ethereal`. 
- Header areas of cards should include a monospaced "Serial Number" or label in the top-right corner to reinforce the developer/architect theme.

### Inputs
- Bottom-border only or fully enclosed with `border-ethereal`. 
- Use `label-mono` for field titles. Focus state should trigger a subtle `secondary-color` blue border and a faint outer glow.

### Chips/Tags
- Monospaced text inside a small, 1px-bordered box with no background, or a very low-opacity blue fill.

### Circular Orbits
- Large, non-interactive decorative strokes that wrap around images or text blocks, adding a "planetary" sense of scale.