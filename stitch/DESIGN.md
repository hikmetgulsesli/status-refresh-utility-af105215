---
name: Precision Utility
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
  on-surface-variant: '#45464d'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#565e74'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#131b2e'
  on-primary-container: '#7c839b'
  inverse-primary: '#bec6e0'
  secondary: '#006c49'
  on-secondary: '#ffffff'
  secondary-container: '#6cf8bb'
  on-secondary-container: '#00714d'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#0b1c30'
  on-tertiary-container: '#75859d'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#d3e4fe'
  tertiary-fixed-dim: '#b7c8e1'
  on-tertiary-fixed: '#0b1c30'
  on-tertiary-fixed-variant: '#38485d'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 30px
    fontWeight: '600'
    lineHeight: 38px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.02em
  label-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '600'
    lineHeight: 14px
    letterSpacing: 0.05em
  code:
    fontFamily: jetbrainsMono
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 20px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  container-max: 1440px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 32px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 24px
---

## Brand & Style

The design system is engineered for high-utility dashboards where clarity and data density must coexist with ease of use. The brand personality is functional, reliable, and unobtrusive—positioning itself as a tool rather than an experience. It targets professional users who require a high degree of "signal-to-noise" ratio.

The style is **Professional Minimalism**. It leverages significant whitespace to prevent cognitive overload, using subtle borders rather than heavy shadows to define structure. The aesthetic prioritizes accessibility and intentionality, ensuring that every element on the screen serves a specific functional purpose. It avoids decorative flourishes in favor of a systematic, "industrial-strength" digital interface.

## Colors

The palette is anchored in a professional, neutral foundation to keep the user's focus on data. 

- **Primary:** A deep Slate (#0F172A) used for high-level navigation, headings, and core brand moments.
- **Secondary (Accent):** Emerald (#10B981) is the "Action" color. It is used exclusively for primary buttons, success states, and active indicators to provide a clear path for the user’s eye.
- **Tertiary:** A muted Slate (#64748B) used for secondary text, icons, and less critical information.
- **Neutral:** A range of cool grays starting from the background (#F8FAFC) up to border tones (#E2E8F0).

Status colors follow standard conventions: Ruby for errors, Amber for warnings, and Blue for informational banners, all calibrated for AA accessibility on white backgrounds.

## Typography

The design system uses **Inter** for all UI elements to ensure maximum legibility across different display resolutions. The typographic scale is tightly controlled to maintain a vertical rhythm.

- **Headlines:** Use semi-bold weights with slight negative letter-spacing to appear grounded and authoritative.
- **Body Text:** Standardized at 14px for data-heavy views (body-md) to allow for higher density without sacrificing readability. 
- **Labels:** Small caps or medium-weight labels are used for table headers and category descriptors to differentiate them from interactive data points.
- **Monospace:** **JetBrains Mono** is introduced for IDs, transaction hashes, or technical data strings to ensure character distinction.

## Layout & Spacing

This design system employs a **Fluid-Fixed Hybrid** model. Navigation and sidebars are fixed in width, while the main content area utilizes a fluid grid that expands to a maximum width of 1440px to prevent excessive line lengths.

- **The 4px Grid:** All measurements (padding, margin, height) must be multiples of 4px.
- **Desktop (1280px+):** 12-column grid, 24px gutters, 32px side margins.
- **Tablet (768px - 1279px):** 8-column grid, 20px gutters, 24px side margins.
- **Mobile (< 767px):** 4-column grid, 16px gutters, 16px side margins.

Structure should be defined by the "Stack" logic: elements within a component use `stack-sm`, components within a section use `stack-md`, and major sections use `stack-lg`.

## Elevation & Depth

Depth in this design system is created through **Low-Contrast Outlines** and tonal variation rather than traditional shadows. This keeps the interface feeling flat and "engineered."

- **Level 0 (Background):** The base layer used for the page body (#F8FAFC).
- **Level 1 (Surface):** The primary container color (White). Used for cards, sidebars, and main content areas. It is defined by a 1px border in color #E2E8F0.
- **Level 2 (Interactive):** Elements that are hoverable or active use a very subtle ambient shadow (0px 1px 3px rgba(0,0,0,0.05)) to suggest "clickability."
- **Overlays:** Modals and dropdowns use a slightly more pronounced shadow (0px 10px 15px -3px rgba(0,0,0,0.1)) and a backdrop blur of 4px to maintain context without visual noise.

## Shapes

The shape language is **Soft** but disciplined. 

- **Standard Elements:** Buttons, input fields, and small tags use a 0.25rem (4px) corner radius. This provides a modern feel without appearing too "playful" or consumer-focused.
- **Containers:** Cards and large panels use 0.5rem (8px). 
- **Icons:** Use a 2px stroke width with rounded ends to match the UI's subtle corner treatment. 

Avoid circles (fully rounded elements) unless used for status indicators or user avatars, as square-off edges better suit a systematic dashboard.

## Components

- **Buttons:** Primary buttons use the secondary color (Emerald) with white text. Secondary buttons use a white background with a 1px border (#E2E8F0).
- **Inputs:** Fields are 40px tall (desktop) with a 1px border. On focus, the border transitions to the primary color or a subtle blue, with a 2px outer "ring" of 10% opacity.
- **Cards:** White background, 1px #E2E8F0 border, no shadow. Card headers should have a bottom border to separate titles from content.
- **Chips/Tags:** Used for status. They should use a "de-saturated" background color (e.g., light green background with dark green text) to be legible but not distracting.
- **Lists/Tables:** Use "zebra-striping" or subtle bottom borders (#F1F5F9). Row hover states should use #F8FAFC.
- **Data Visualizations:** Use the primary palette for charts. Avoid gradients in data; use solid, high-contrast fills for clarity.
- **Navigation:** The sidebar should use a high-contrast theme (Slate #0F172A) to clearly separate the application structure from the workspace.