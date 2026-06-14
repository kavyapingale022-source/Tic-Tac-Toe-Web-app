---
name: Hyperion Protocol
colors:
  surface: '#121318'
  surface-dim: '#121318'
  surface-bright: '#38393f'
  surface-container-lowest: '#0d0e13'
  surface-container-low: '#1a1b21'
  surface-container: '#1e1f25'
  surface-container-high: '#292a2f'
  surface-container-highest: '#34343a'
  on-surface: '#e3e1e9'
  on-surface-variant: '#b9cacb'
  inverse-surface: '#e3e1e9'
  inverse-on-surface: '#2f3036'
  outline: '#849495'
  outline-variant: '#3b494b'
  surface-tint: '#00dbe9'
  primary: '#dbfcff'
  on-primary: '#00363a'
  primary-container: '#00f0ff'
  on-primary-container: '#006970'
  inverse-primary: '#006970'
  secondary: '#ecb2ff'
  on-secondary: '#520071'
  secondary-container: '#cf5cff'
  on-secondary-container: '#480063'
  tertiary: '#fff3f4'
  on-tertiary: '#66002c'
  tertiary-container: '#ffccd6'
  on-tertiary-container: '#bb0058'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#7df4ff'
  primary-fixed-dim: '#00dbe9'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#f8d8ff'
  secondary-fixed-dim: '#ecb2ff'
  on-secondary-fixed: '#320047'
  on-secondary-fixed-variant: '#74009f'
  tertiary-fixed: '#ffd9e0'
  tertiary-fixed-dim: '#ffb1c3'
  on-tertiary-fixed: '#3f0019'
  on-tertiary-fixed-variant: '#8f0041'
  background: '#121318'
  on-background: '#e3e1e9'
  surface-variant: '#34343a'
typography:
  display-xl:
    fontFamily: Sora
    fontSize: 72px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Sora
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Sora
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Sora
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
    lineHeight: '1.6'
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.4'
    letterSpacing: 0.05em
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.4'
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
  container-padding: 40px
  gutter: 24px
  stack-sm: 12px
  stack-md: 24px
  stack-lg: 48px
---

## Brand & Style

This design system is a fusion of high-fidelity spatial computing and neon-infused gaming aesthetics. It targets a premium audience that values immersion, technical precision, and sensory-rich interfaces. The emotional response should be one of "controlled energy"—the excitement of a high-stakes digital environment balanced by the sleek, intuitive usability of a luxury operating system.

The design style is **Glassmorphism / Futuristic-Tech**. It utilizes heavy backdrop blurs, translucent layers, and vibrant light-source simulations to create a sense of physical depth. Elements should feel like they are floating in a 3D space, illuminated by internal power sources and peripheral neon pulses.

## Colors

The palette is anchored in a "Deep Space" foundation to provide maximum contrast for neon accents. 

- **Primary (Electric Cyan):** Used for critical actions, active states, and primary energy paths.
- **Secondary (Phlox Purple):** Used for leveling, progression elements, and secondary highlights.
- **Tertiary (Neon Pink):** Reserved for alerts, rare items, or high-intensity UI moments.
- **Surface Neutrals:** Not pure black, but deep tinted navy to maintain a sense of atmospheric volume.

Gradients should primarily flow from Secondary to Primary to create a "charging" visual effect.

## Typography

The typography strategy balances geometric personality with technical utility. 
- **Sora** is the display powerhouse, providing a futuristic, wide-set stance for headlines.
- **Inter** handles all long-form reading and core UI text to ensure maximum legibility against complex glass backgrounds.
- **JetBrains Mono** is used for "Data-Ink"—stats, coordinates, and system readouts—reinforcing the cyberpunk/hacker aesthetic.

All labels should be set in Uppercase when used for navigation or technical categories to enhance the "heads-up display" (HUD) feel.

## Layout & Spacing

This design system uses a **Fluid Spatial Grid**. Rather than rigid columns, elements are treated as floating modules within a 3D-aware canvas.

- **Desktop:** 12-column grid with wide margins (40px+) to allow the background particles and glows to breathe.
- **Safe Zones:** High-priority HUD elements (user profile, currency, navigation) are pinned to corners with a 32px safe-area offset.
- **Depth Stacking:** Spacing is not just horizontal and vertical, but Z-axis. Use 24px increments for element separation to suggest airiness.

## Elevation & Depth

Depth is the core differentiator of this design system. It is achieved through three specific layers:

1.  **The Void (Background):** A deep gradient from `#020308` to `#0A0B10`, populated with subtle floating particles.
2.  **The Glass (Midground):** Translucent cards with a 20px to 40px backdrop blur. Each card must feature a 1px "specular edge"—a subtle inner stroke (`rgba(255,255,255,0.15)`) on the top and left sides to simulate light catching the glass edge.
3.  **The Glow (Foreground):** Active elements emit a soft outer glow (drop-shadow with 20px+ blur) in the primary or secondary color.

Use **Inner Shadows** (top-down) to create an "etched" look for input fields and containers, making them look like they are carved into the glass.

## Shapes

The shape language is sophisticated and "hyper-rounded." While the base roundedness is set to `2`, significant containers (cards, modals) should utilize `rounded-2xl` (24px) or `rounded-3xl` (32px) to mimic the organic feel of modern spatial hardware.

Interactive elements like buttons and chips should remain highly rounded (Pill-shaped) to provide a friendly, tactile contrast to the sharp, technical typography.

## Components

- **Buttons:** Primary buttons use a vibrant gradient (Cyan to Purple) with a white `label-md` font. Hover states should trigger an increase in glow intensity rather than a color change.
- **Glass Cards:** Must have a `backdrop-filter: blur(30px)` and a thin, semi-transparent border. Content inside should have ample padding (32px+) to maintain the premium feel.
- **Inputs:** Dark, recessed backgrounds with a bright 1px bottom border that "activates" (glows) when focused.
- **Chips/Badges:** Small, pill-shaped elements with high-contrast fills (e.g., a "Rare" item badge in Tertiary Pink).
- **Progress Bars:** Use a neon "pulse" animation—a highlight stripe that travels across the filled portion of the bar to indicate active energy.
- **HUD Nav:** A floating bottom bar, detached from the screen edge, using the maximum glass effect and rounded-full corners.