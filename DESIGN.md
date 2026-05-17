---
name: Lumen Essentials
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1b1b1b'
  surface-container: '#1f1f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353535'
  on-surface: '#e2e2e2'
  on-surface-variant: '#c4c7c8'
  inverse-surface: '#e2e2e2'
  inverse-on-surface: '#303030'
  outline: '#8e9192'
  outline-variant: '#444748'
  surface-tint: '#c6c6c7'
  primary: '#ffffff'
  on-primary: '#2f3131'
  primary-container: '#e2e2e2'
  on-primary-container: '#636565'
  inverse-primary: '#5d5f5f'
  secondary: '#c7c6c6'
  on-secondary: '#303031'
  secondary-container: '#464747'
  on-secondary-container: '#b5b5b5'
  tertiary: '#ffffff'
  on-tertiary: '#2f3131'
  tertiary-container: '#e2e2e2'
  on-tertiary-container: '#636565'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e2e2e2'
  primary-fixed-dim: '#c6c6c7'
  on-primary-fixed: '#1a1c1c'
  on-primary-fixed-variant: '#454747'
  secondary-fixed: '#e3e2e2'
  secondary-fixed-dim: '#c7c6c6'
  on-secondary-fixed: '#1b1c1c'
  on-secondary-fixed-variant: '#464747'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c7'
  on-tertiary-fixed: '#1a1c1c'
  on-tertiary-fixed-variant: '#454747'
  background: '#131313'
  on-background: '#e2e2e2'
  surface-variant: '#353535'
typography:
  display-xl:
    fontFamily: Geist
    fontSize: 80px
    fontWeight: '700'
    lineHeight: 80px
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Geist
    fontSize: 28px
    fontWeight: '600'
    lineHeight: 36px
  body-md:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.05em
spacing:
  unit: 8px
  container-padding: 24px
  element-gap: 16px
  section-margin: 48px
---

## Brand & Style

The design system is built on the principle of absolute functionalism. It serves as a literal mirror to the environment it measures, utilizing a monochromatic spectrum to represent the transition from total darkness to peak luminosity. 

The aesthetic is **Minimalist** with **High-Contrast** accents. By stripping away all chromatic noise, the user can focus entirely on the core data: light intensity. The interface relies on stark voids and brilliant fills to evoke a sense of precision and utility. It is intended for professional and hobbyist use in cinematography, interior design, and botany, where legibility in extreme lighting conditions is paramount.

## Colors

The palette is strictly achromatic. 
- **Primary:** Pure White (#FFFFFF) is used for active light readings, primary text, and the "fill" of data visualizations.
- **Neutral:** Pure Black (#000000) serves as the canvas, ensuring maximum contrast and reducing screen glare in dark environments.
- **Secondary:** A mid-tone Grey (#888888) is used for inactive states, secondary labels, and UI scaffolding.

The color logic is direct: higher lux levels translate to more white surface area; lower lux levels allow the black canvas to dominate.

## Typography

This design system utilizes **Geist** for its technical precision and neutral character. It ensures that numerical data is clear and authoritative. To provide a "utility tool" feel, **JetBrains Mono** is introduced for metadata and labels, reinforcing the feeling of a scientific instrument.

- **Display XL:** Reserved exclusively for the central Lux value.
- **Labels:** Set in uppercase monospaced type to distinguish supplemental data from primary readings.
- **Weighting:** Use Bold (700) for readings and Regular (400) for instructional text.

## Layout & Spacing

The layout follows a **Fixed Grid** model centered on a vertical axis. On mobile, the interface is divided into three zones:
1. **Header:** Minimal metadata (e.g., sensor status).
2. **Hero:** A large, square central area dedicated to the circular lux meter.
3. **Control/Data:** A bottom-weighted section for secondary readings (Min/Max/Avg) and history.

Spacing is generous to prevent accidental taps and to ensure that the primary visualization remains the focal point. Elements are separated by large voids to maintain the minimalist integrity.

## Elevation & Depth

Depth is conveyed through **Low-Contrast Outlines** rather than shadows. In a monochromatic dark mode, shadows are ineffective. Instead, layers are defined by:
- **Stroke Contrast:** Elements are contained within 1px white or grey borders.
- **Opacity:** Dimmed layers (e.g., background grids) use 10-20% opacity white lines over the black background.
- **Physicality:** The design avoids "floating" elements, preferring a flat, "printed-to-glass" look where hierarchy is determined by stroke weight and font size.

## Shapes

The design system adopts a **Sharp (0)** roundedness strategy. Square corners emphasize the technical, "instrumentation" nature of the app. Circles are only permitted for the primary data visualization (the Lux meter) and toggle switches, creating a clear visual distinction between data containers and interactive controls.

## Components

### Lux Meter (Primary)
The centerpiece. A circular progress bar with a 24px stroke weight. The "track" is dark grey (#222222), and the "indicator" is pure white (#FFFFFF). The numerical value sits in the center in `display-xl`.

### Buttons
Primary buttons are solid white with black text. Secondary buttons are outlined (1px white) with no fill. All buttons use sharp 0px corners.

### Data Cards
Simple black boxes with 1px grey borders. These display secondary metrics like "MAX" or "AVG". Labels are positioned at the top-left of the card in `label-mono`.

### Input Fields
Underlined only (not boxed). The line is 1px white. Focus state is indicated by a thickness increase to 2px.

### List Items
Separated by 1px grey hairline dividers that span the full width of the container. No icons are used unless strictly necessary for functionality.