---
name: Machine Experience (MX)
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#20201f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353535'
  on-surface: '#e5e2e1'
  on-surface-variant: '#cfc4c5'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#988e90'
  outline-variant: '#4c4546'
  surface-tint: '#c6c6c6'
  primary: '#c6c6c6'
  on-primary: '#303030'
  primary-container: '#000000'
  on-primary-container: '#757575'
  inverse-primary: '#5e5e5e'
  secondary: '#c6c6c7'
  on-secondary: '#2f3131'
  secondary-container: '#454747'
  on-secondary-container: '#b4b5b5'
  tertiary: '#c6c6c6'
  on-tertiary: '#303030'
  tertiary-container: '#000000'
  on-tertiary-container: '#757575'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e2e2e2'
  primary-fixed-dim: '#c6c6c6'
  on-primary-fixed: '#1b1b1b'
  on-primary-fixed-variant: '#474747'
  secondary-fixed: '#e2e2e2'
  secondary-fixed-dim: '#c6c6c7'
  on-secondary-fixed: '#1a1c1c'
  on-secondary-fixed-variant: '#454747'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1b1b1b'
  on-tertiary-fixed-variant: '#474747'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353535'
typography:
  display:
    fontFamily: Inter
    fontSize: 80px
    fontWeight: '700'
    lineHeight: '1.0'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '600'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '500'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0em
  body-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0em
  label-caps:
    fontFamily: Space Grotesk
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.1em
  mono-technical:
    fontFamily: Space Grotesk
    fontSize: 13px
    fontWeight: '400'
    lineHeight: '1.4'
    letterSpacing: 0em
spacing:
  unit: 4px
  gutter: 24px
  margin-page: 64px
  section-gap: 160px
  container-max: 1440px
---

## Brand & Style

This design system is engineered to evoke a "Machine Experience" (MX)—a state of hyper-precision where human creativity meets algorithmic accuracy. The brand personality is cold, intellectual, and uncompromisingly efficient, designed for a high-tier AI design agency. It prioritizes the "technical yet elegant" aesthetic through a synthesis of high-modern minimalism and subtle glassmorphism. 

The emotional response should be one of "quiet power." By stripping away decorative clutter and relying on generous white space and thin, razor-sharp borders, the UI communicates that the intelligence behind the interface is sophisticated enough to be invisible. Transitions are not just decorative but functional, mimicking the smooth, low-latency processing of a high-end machine.

## Colors

The palette is strictly monochromatic to maintain a laboratory-grade focus on content and data. The default mode is deep dark, utilizing absolute black (#000000) to create a void-like depth. 

- **Primary & Secondary:** Absolute black and white provide the highest possible contrast for core structural elements.
- **Grays:** Light grays are used sparingly for secondary text and subtle borders, ensuring the hierarchy is felt rather than seen.
- **Accent:** A single, high-precision blue or white-glow is reserved exclusively for interactivity (hover states, active indicators, or progress bars) to signal machine "life" without breaking the monochrome discipline.

## Typography

This design system employs high-contrast typography to create an editorial feel within a technical framework. **Inter** provides the utilitarian foundation for body and headlines, while **Space Grotesk** is introduced for labels and technical data to reinforce the "machine" aesthetic.

Large-scale display type should be set with tight tracking to appear like a physical block of text. Smaller labels should be generously tracked out and set in all-caps to act as navigational markers. Hierarchy is achieved through size disparity rather than excessive weight variation.

## Layout & Spacing

The layout philosophy follows a **fixed grid** with extreme internal breathing room. A 12-column grid is used, but content is often pushed to the center or aligned to the edges to create asymmetric tension. 

The "section-gap" is intentionally large to force the user to focus on one concept at a time. Spacing rhythm is strictly mathematical, based on a 4px baseline grid. Use whitespace as a structural element to separate functional zones rather than relying on heavy containers or background changes.

## Elevation & Depth

Depth in this design system is created through **Glassmorphism and Tonal Layering** rather than traditional shadows. 

1.  **Base Layer:** Absolute Black (#000000).
2.  **Surface Layer:** Semi-transparent dark grays with a high-density `backdrop-filter: blur(20px)`.
3.  **Borders:** 1px solid borders using low-opacity white (e.g., `rgba(255, 255, 255, 0.1)`) create the illusion of glass edges.

Avoid shadows entirely. If depth is required for a floating element, use a subtle 1px inner stroke to "catch the light" on the top edge, simulating a physical, machined object.

## Shapes

The shape language is **Sharp (0)**. To convey precision and an industrial machine quality, all corners are 90 degrees. No radii are permitted on buttons, cards, or input fields. 

This architectural rigidity is softened by the use of translucent materials and smooth motion, ensuring the interface feels modern rather than dated. Small, decorative elements like "crosshair" icons or corner-bracket accents can be used to frame content areas, reinforcing the technical drafting feel.

## Components

- **Buttons:** Rectangular with 1px white borders. Fill is transparent. On hover, the button fills with solid white and flips text to black with a 200ms ease-out transition.
- **Inputs:** Minimalist bottom-border only. Labels are set in `label-caps` above the field. Focus state triggers a subtle glow on the bottom border.
- **Cards:** Defined by thin 1px borders and backdrop blurs. No background color change from the main surface unless nested.
- **Chips/Tags:** Monospaced text wrapped in brackets, e.g., `[PROCESS_01]`, rather than pill shapes.
- **Transitions:** Use "linear" or "circ-out" easing for motion. Elements should slide or fade with machine-like rigidity.
- **Cursors:** Custom 10px circular "target" cursor with a subtle inversion effect over text.
- **Data Indicators:** Vertical bars and thin line charts to represent AI activity or system status.