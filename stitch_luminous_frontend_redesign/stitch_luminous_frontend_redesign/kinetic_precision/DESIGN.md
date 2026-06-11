---
name: Kinetic Precision
colors:
  surface: '#faf8ff'
  surface-dim: '#d2d9f4'
  surface-bright: '#faf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f3ff'
  surface-container: '#eaedff'
  surface-container-high: '#e2e7ff'
  surface-container-highest: '#dae2fd'
  on-surface: '#131b2e'
  on-surface-variant: '#3b494c'
  inverse-surface: '#283044'
  inverse-on-surface: '#eef0ff'
  outline: '#6b7a7d'
  outline-variant: '#bac9cc'
  surface-tint: '#006875'
  primary: '#006875'
  on-primary: '#ffffff'
  primary-container: '#00e5ff'
  on-primary-container: '#00626e'
  inverse-primary: '#00daf3'
  secondary: '#006c49'
  on-secondary: '#ffffff'
  secondary-container: '#6cf8bb'
  on-secondary-container: '#00714d'
  tertiary: '#9d4300'
  on-tertiary: '#ffffff'
  tertiary-container: '#ffc4a6'
  on-tertiary-container: '#953f00'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#9cf0ff'
  primary-fixed-dim: '#00daf3'
  on-primary-fixed: '#001f24'
  on-primary-fixed-variant: '#004f58'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#ffdbca'
  tertiary-fixed-dim: '#ffb690'
  on-tertiary-fixed: '#341100'
  on-tertiary-fixed-variant: '#783200'
  background: '#faf8ff'
  on-background: '#131b2e'
  surface-variant: '#dae2fd'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-sm:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.05em
  data-lg:
    fontFamily: Hanken Grotesk
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 32px
---

## Brand & Style

The design system is engineered for high-stakes telemetry monitoring where cognitive load must be minimized. The brand personality is **analytical, responsive, and technical**, evoking the feeling of a professional-grade aerospace or automotive diagnostic suite. It prioritizes utility and rapid data ingestion over decorative flair.

The visual style is a **Modern "Pro-Tool"** aesthetic. It moves away from the dark, gamer-centric tones of standard telemetry and adopts a sophisticated light-mode interface characterized by:
- **High Information Density:** Compact layouts that maximize screen real estate without feeling cluttered.
- **Micro-Precision:** Fine 1px borders and subtle hairline dividers to separate complex data sets.
- **Functional Color Theory:** Using color only to signify status, performance metrics, or alerts, ensuring that "everything that is colored has a meaning."
- **Institutional Clarity:** A foundation of crisp whites and architectural grays to provide a neutral stage for vibrant data visualizations.

## Colors

This design system utilizes a high-contrast light palette designed for readability under various lighting conditions.

- **Primary (Electric Cyan):** Reserved for active performance data, motion, speed, and primary action indicators. It represents the "flow" of energy.
- **Secondary (Vibrant Green):** Dedicated to battery health, "Good" status indicators, and successful system connections.
- **Tertiary (Safety Orange/Red):** Used exclusively for warnings, critical faults, and values exceeding safe thresholds (#F43F5E for errors).
- **Neutrals:** A range of Slate grays provides the structural framework. Surface backgrounds use a very light cool gray to reduce screen glare while keeping the primary content areas pure white.
- **Data Visualization:** Use a sequence of secondary colors for charts (e.g., Indigo, Violet) only when distinguishing between multiple overlapping data streams.

## Typography

Typography is treated as a functional component. 
- **Hanken Grotesk** is the workhorse font, chosen for its contemporary geometric construction which remains legible at small sizes and high weights.
- **JetBrains Mono** is used for technical labels, timestamps, and raw sensor output (coordinates, UUIDs). The monospaced nature ensures that fluctuating numerical data doesn't cause "jitter" in the layout.
- **Data Roles:** Large numerical readouts (e.g., speed, SOC) use the `data-lg` role with tight letter spacing to emphasize the specific value.
- **All-Caps:** Use all-caps sparingly, primarily for `label-md` roles to denote section categories or sensor names.

## Layout & Spacing

The layout utilizes a **12-column fluid grid** for desktop and a **4-column grid** for mobile. 

- **Modular Blocks:** Data is contained within modular "cards" or "widgets" that span 3, 4, 6, or 12 columns depending on the complexity of the visualization.
- **Rhythm:** An 8px (2-unit) base increment drives all spacing. For tight technical data, 4px (1-unit) padding is permitted within components.
- **Density:** This system favors a "Medium-High" density. Information is grouped logically with `16px` gutters, while `24px` or `32px` margins separate major logical sections (e.g., "Vehicle Status" vs "Live Tracking").
- **Alignment:** All data labels must be top-aligned or left-aligned; center alignment is only permitted for primary circular gauges.

## Elevation & Depth

To maintain a "pro-tool" feel, this design system avoids heavy shadows and skeuomorphism. Depth is communicated through **Tonal Layering and Outlines**:

- **Floor:** The application background is `#F8FAFC`.
- **Level 1 (Cards):** Primary containers are pure white (`#FFFFFF`) with a 1px solid border (`#E2E8F0`).
- **Level 2 (Insets):** Search bars, input fields, or nested data groups use a subtle inset feel with a light gray fill (`#F1F5F9`).
- **Stateful Depth:** Hovering over an interactive widget should trigger a very soft, diffused shadow (`0 4px 12px rgba(15, 23, 42, 0.05)`) to indicate interactivity.
- **Dividers:** Horizontal and vertical rules should be `1px` and use the border color, ensuring they never compete with the text for attention.

## Shapes

The shape language is **Soft (0.25rem)**. This provides a professional, "industrial-modern" look that feels engineered rather than playful.

- **Standard Radius:** 4px for buttons, input fields, and small tags.
- **Large Radius:** 8px (`rounded-lg`) for primary data cards and map containers.
- **Pills:** Only used for status indicators (e.g., "Connected", "Live") to make them instantly recognizable as non-interactive status badges.
- **Interactive Elements:** Buttons maintain the standard 4px radius to distinguish them from the purely informational status pills.

## Components

- **Buttons:** Primary buttons use the Cyan base with dark text. Ghost buttons use the border color and primary text for secondary actions like "Export Data."
- **Status Chips:** Small, pill-shaped badges. Use a light tinted background (10% opacity) of the functional color with a high-contrast dark label (e.g., Light Green BG + Dark Green Text).
- **Data Cards:** Every card must have a `label-md` header. The primary value should be in `data-lg`. If a trend exists, place a small sparkline or percentage change indicator in the bottom right corner.
- **Input Fields:** 1px border, 4px radius. On focus, the border changes to Primary Cyan with a 2px outer glow.
- **Progress Bars / Gauges:** Use clean, un-textured fills. For circular gauges, use a thin track and a thick indicator to emphasize the current value.
- **Telemetry Lists:** Use zebra-striping (alternating `#F8FAFC` and `#FFFFFF`) for long lists of sensor logs to assist horizontal eye tracking.