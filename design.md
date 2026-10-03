---
name: Resonant Stark
colors:
  surface: '#fbf8ff'
  surface-dim: '#dcd9e0'
  surface-bright: '#fbf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f6f2fa'
  surface-container: '#f0ecf4'
  surface-container-high: '#eae7ee'
  surface-container-highest: '#e4e1e9'
  on-surface: '#1b1b20'
  on-surface-variant: '#4c4451'
  inverse-surface: '#303035'
  inverse-on-surface: '#f3eff7'
  outline: '#7d7482'
  outline-variant: '#cec3d2'
  surface-tint: '#7a45a9'
  primary: '#2f0052'
  on-primary: '#ffffff'
  primary-container: '#4a0e78'
  on-primary-container: '#b981ea'
  inverse-primary: '#dfb7ff'
  secondary: '#841cd8'
  on-secondary: '#ffffff'
  secondary-container: '#9e42f2'
  on-secondary-container: '#fffbff'
  tertiary: '#2b0a46'
  on-tertiary: '#ffffff'
  tertiary-container: '#42225d'
  on-tertiary-container: '#af8bcd'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#f1daff'
  primary-fixed-dim: '#dfb7ff'
  on-primary-fixed: '#2d004f'
  on-primary-fixed-variant: '#612b8f'
  secondary-fixed: '#f0dbff'
  secondary-fixed-dim: '#ddb7ff'
  on-secondary-fixed: '#2c0050'
  on-secondary-fixed-variant: '#6900b3'
  tertiary-fixed: '#f1daff'
  tertiary-fixed-dim: '#dfb7fd'
  on-tertiary-fixed: '#2b0945'
  on-tertiary-fixed-variant: '#593874'
  background: '#fbf8ff'
  on-background: '#1b1b20'
  surface-variant: '#e4e1e9'
typography:
  headline-xl:
    fontFamily: Montserrat
    fontSize: 64px
    fontWeight: '900'
    lineHeight: '1.1'
    letterSpacing: 0.05em
  headline-lg:
    fontFamily: Montserrat
    fontSize: 40px
    fontWeight: '900'
    lineHeight: '1.2'
    letterSpacing: 0.02em
  headline-md:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: '900'
    lineHeight: '1.2'
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
  code-label:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.4'
    letterSpacing: 0.02em
  metric-display:
    fontFamily: JetBrains Mono
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.1'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 24px
  margin: 32px
  trace-offset: 12px
---

## Brand & Style
The design system for this electrical engineering firm is built upon the "Resonant Stark" aesthetic—a fusion of neoclassical engraving precision and the raw, functional power of modern electrical infrastructure. The visual language is "Light-First," transitioning from a high-tech underground authority to a clear, clinical, and high-visibility engineering environment, similar to a brightly lit laboratory or a fresh technical schematic.

The style is a hybrid of **Brutalism** and **Technical Schematic Design**. It utilizes heavy 2px strokes to mimic technical ink drawings, PCB circuit traces, and Euclidean geometry. Every interface element is treated as a component within a complex orthogonal plan, ensuring the UI feels engineered rather than merely decorated. The emotional response is one of absolute reliability, precision, and architectural scale.

## Colors
This system operates on a high-contrast, light-centric foundation, prioritizing clarity and legibility.

- **Primary Canvas:** The background is now light, using neutral surfaces to provide a clean slate for technical details.
- **Action Tier:** `brand-primary` (#4A0E78) is reserved for high-priority CTA elements and structural headers. `brand-secondary` (#8E2DE2) acts as the "active circuit" accent for status indicators, hover states, or active circuit paths.
- **Ink & Structure:** `tech-ink` (#111116) is the absolute baseline for typography and the heavy 2px borders that define the layout's structural integrity.
- **High Visibility:** While light-centric, the design maintains deep contrast to ensure schematics are readable in high-glare environments.

## Typography
Typography is treated as an engineering spec. 

- **Headlines:** Montserrat (Black/900) in all-caps creates an authoritative, institutional presence. It should feel "stamped" onto the interface like a physical nameplate.
- **Body:** Inter provides a clean, neutral contrast to the aggressive headings, ensuring legibility for technical specifications and reports.
- **Data & Metrics:** JetBrains Mono is used for all technical data, measurements (V, A, Hz), and status labels, reinforcing the "monospaced" precision of an oscilloscope or terminal.

## Layout & Spacing
The layout follows a **Strict Orthogonal Grid**. It mimics the logic of a PCB (Printed Circuit Board) where elements are connected by logical paths.

- **The Grid:** A 12-column system for desktop with heavy technical vertical dividers to visualize the grid structure.
- **Trace Patterns:** Use 45-degree angled "trace" lines (2px width) to connect disparate content blocks, simulating electrical pathways.
- **Breakpoints:** 
  - **Mobile (<768px):** Single column, 16px margins, vertical stacking of all schematic elements.
  - **Tablet (768px - 1024px):** 6-column grid, 24px margins.
  - **Desktop (>1024px):** Full 12-column schematic with lateral technical annotations in the margins.

## Elevation & Depth
This system rejects soft shadows and "natural" lighting. Depth is communicated through **Structural Brutalism**:

- **Hard Shadows:** Use a fixed `4px 4px 0px #111116` box-shadow on all cards, buttons, and input fields. This gives the UI a physical, "bolted-down" quality against the light background.
- **Tonal Stacking:** Use light neutral tones for the bottom-most layer. Surfaces that "rise" toward the user become pure white or `brand-tint`, but always maintain the thick 2px `tech-ink` border.
- **Schematic Overlays:** Use low-opacity `tech-grid` lines (1px) as a background texture to suggest a blueprint layer beneath the active UI.

## Shapes
Shapes are geometric and rigid. All interactive containers and decorative elements use a consistent **4px (0.25rem)** corner radius. This is enough to prevent the UI from feeling sharp and "hostile" while maintaining the technical precision of a machine-milled component. 

Decorative shapes should include 45-degree chamfered corners for special badges or circuit-node callouts.

## Components

### Buttons
- **Primary:** `brand-primary` background, white text, 2px `tech-ink` border, 4px hard shadow.
- **Action State:** On click, the button shifts +2px down and +2px right, removing the shadow to simulate a physical "press."

### Input Fields
- **Base:** White background, 2px `tech-ink` border. 
- **Focus:** Border changes to `brand-secondary` with a subtle outer glow, simulating a powered-on circuit.

### Cards & Containers
- **Technical Card:** White background with a mandatory 2px `tech-ink` border. Header sections of cards should be separated by a horizontal 2px line.
- **Annotation Badge:** Use `jetbrainsMono` text inside a chamfered-edge container with a technical steel border.

### Status Indicators
- **Active/Live:** `brand-secondary` pulsing dot (simulating power).
- **Static/Off:** `tech-ink` solid dot at reduced opacity.

### PCB Circuit Traces
- Use decorative 2px lines that "bend" at 45-degree angles to lead the eye from one component to another, or to connect a label to its corresponding data point.