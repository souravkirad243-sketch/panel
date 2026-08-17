---
name: CARD//VAULT
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
  on-surface-variant: '#baccb0'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#85967c'
  outline-variant: '#3c4b35'
  surface-tint: '#2ae500'
  primary: '#efffe3'
  on-primary: '#053900'
  primary-container: '#39ff14'
  on-primary-container: '#107100'
  inverse-primary: '#106e00'
  secondary: '#dcfdff'
  on-secondary: '#00373a'
  secondary-container: '#00f1fd'
  on-secondary-container: '#006a6f'
  tertiary: '#fff8fe'
  on-tertiary: '#470083'
  tertiary-container: '#ebd5ff'
  on-tertiary-container: '#8900f5'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#79ff5b'
  primary-fixed-dim: '#2ae500'
  on-primary-fixed: '#022100'
  on-primary-fixed-variant: '#095300'
  secondary-fixed: '#6ff6ff'
  secondary-fixed-dim: '#00dce6'
  on-secondary-fixed: '#002022'
  on-secondary-fixed-variant: '#004f53'
  tertiary-fixed: '#efdbff'
  tertiary-fixed-dim: '#dab9ff'
  on-tertiary-fixed: '#2b0053'
  on-tertiary-fixed-variant: '#6500b8'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-lg:
    fontFamily: Geist
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  display-lg-mobile:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '800'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: -0.01em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  technical-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.5'
    letterSpacing: 0.05em
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 10px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  xs: 8px
  sm: 16px
  md: 24px
  lg: 40px
  xl: 80px
  gutter: 20px
  margin-mobile: 16px
  margin-desktop: 64px
---

## Brand & Style
The design system for this product is a premium, high-fidelity interpretation of the "Cyberpunk" aesthetic, shifting away from "low-life" grit toward "high-tech" sophistication. It targets high-end collectors and traders who value technical precision and digital security. 

The visual direction combines **Minimalism** with **Glassmorphism** and **High-Contrast** accents. The UI should evoke the feeling of a secure, encrypted terminal—clean, authoritative, and fast. Key stylistic signatures include:
- **Luminance over Surface:** Depth is defined by light emissions (glows) rather than traditional shadows.
- **Data-Density:** Using monospaced microcopy to provide a "technical" feel without sacrificing usability.
- **Scanning Textures:** Subtle 1px grid overlays and scan-line patterns on backgrounds to reinforce the digital vault metaphor.

## Colors
The palette is rooted in deep blacks to maximize the "pop" of the neon accents. 

- **Primary (Neon Green):** Reserved for primary actions and success states. It represents "Go" or "Active."
- **Secondary (Cyan):** Used for information, focus states, and iconography. It represents "Data" or "System."
- **Tertiary (Purple):** Used sparingly for rare items, highlights, or secondary interactive states.
- **Backgrounds:** The base layer is `#050505`. Interactive surfaces and containers use `#121212` to create a tiered hierarchy of information.

## Typography
The typography system uses a dual-axis approach. **Geist** and **Inter** handle the core UX, ensuring high readability and a modern, professional feel. **JetBrains Mono** is utilized for "Terminal Details"—serial numbers, price fluctuations, timestamps, and technical specifications—to ground the design in its cyberpunk narrative.

Headlines should be tight and impactful. Large display text should occasionally use a "glitch" or "slice" effect in marketing contexts. All technical microcopy should be set in monospaced fonts with increased letter spacing for a hardware-interface aesthetic.

## Layout & Spacing
The layout follows a **Fluid Grid** model with high horizontal margins to create a "contained" feel, as if viewing a secure console.

- **Desktop:** 12-column grid with 20px gutters. Content is often centered with a max-width of 1440px.
- **Tablet:** 8-column grid with 16px gutters.
- **Mobile:** 4-column grid with 16px margins.

Spacing should be rigid and mathematical, using multiples of 4px. Avoid "soft" or organic spacing; elements should feel snapped to a technical grid.

## Elevation & Depth
In this design system, depth is achieved through **Tonal Layers** and **Light Emission** rather than shadow casting.

- **Level 0 (Background):** `#050505` with a subtle 4% opacity grid overlay.
- **Level 1 (Card/Surface):** `#121212` with a 1px solid border of `rgba(255, 255, 255, 0.05)`.
- **Level 2 (Active/Hover):** Glassmorphic background blur (20px) with a subtle secondary color glow (`#00F3FF`) at 10-15% opacity.
- **Interactive Depth:** When an element is focused, use a "Cyan Glow" (`box-shadow: 0 0 15px rgba(0, 243, 255, 0.3)`) to indicate life.

## Shapes
The shape language is "Aggressive-Precision." While a pure 0px radius is too brutalist for a premium e-commerce site, a **2px radius (Soft)** is used for all buttons, inputs, and cards. This creates a "machined" look—sharp enough to feel high-tech, but refined enough to feel professional.

- **Standard Radius:** 2px.
- **Outer Container Radius:** 4px (used only for large page wrappers or main modal containers).
- **Icons:** Should use square terminals rather than rounded caps to match the font geometry.

## Components

### Buttons
- **Primary:** Neon Green (`#39FF14`) background, black text. On hover, add a `0 0 20px` neon green outer glow.
- **Secondary:** Outline only. Cyan (`#00F3FF`) 1px border with cyan text. On hover, the background fills with 10% cyan opacity.
- **Ghost:** Monospaced text with a `> ` prefix to mimic a command line prompt.

### Cards (The "Vault" Item)
- Deep charcoal surface (`#121212`).
- 1px border in `rgba(0, 243, 255, 0.1)`.
- Image area: High-tech card visuals should have a subtle drop-shadow using the card's dominant color to simulate a holographic projection.

### Input Fields
- Minimalist underline or 1px border. Background is slightly darker than the surface.
- Focus state: Border color changes to Cyan with a faint "beam" glow.
- Placeholder text: Set in JetBrains Mono at 40% opacity.

### Icons
- Use 1.5px stroke weight.
- Always Cyan (`#00F3FF`) or white.
- Icons should be housed in a small square container with a subtle 1px border to look like "HUD" elements.

### Progress Bars / Status
- Use a "segmented" loading bar (blocks instead of a smooth line) to reinforce the technical, retro-future feel.