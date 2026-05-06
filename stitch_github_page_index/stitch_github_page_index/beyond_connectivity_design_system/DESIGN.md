---
name: Beyond Connectivity Design System
colors:
  surface: '#fbf9f8'
  surface-dim: '#dcd9d9'
  surface-bright: '#fbf9f8'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f6f3f2'
  surface-container: '#f0eded'
  surface-container-high: '#eae8e7'
  surface-container-highest: '#e4e2e1'
  on-surface: '#1b1c1c'
  on-surface-variant: '#594140'
  inverse-surface: '#303030'
  inverse-on-surface: '#f3f0f0'
  outline: '#8d706f'
  outline-variant: '#e1bebd'
  surface-tint: '#b22933'
  primary: '#7e0016'
  on-primary: '#ffffff'
  primary-container: '#a11c29'
  on-primary-container: '#ffb3b1'
  inverse-primary: '#ffb3b1'
  secondary: '#4f6073'
  on-secondary: '#ffffff'
  secondary-container: '#d2e4fb'
  on-secondary-container: '#556679'
  tertiary: '#3c3c39'
  on-tertiary: '#ffffff'
  tertiary-container: '#545350'
  on-tertiary-container: '#c9c6c3'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdad8'
  primary-fixed-dim: '#ffb3b1'
  on-primary-fixed: '#410007'
  on-primary-fixed-variant: '#900b1f'
  secondary-fixed: '#d2e4fb'
  secondary-fixed-dim: '#b7c8de'
  on-secondary-fixed: '#0b1d2d'
  on-secondary-fixed-variant: '#38485a'
  tertiary-fixed: '#e5e2de'
  tertiary-fixed-dim: '#c8c6c2'
  on-tertiary-fixed: '#1c1c19'
  on-tertiary-fixed-variant: '#474744'
  background: '#fbf9f8'
  on-background: '#1b1c1c'
  surface-variant: '#e4e2e1'
typography:
  h1:
    fontFamily: Manrope
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  h2:
    fontFamily: Manrope
    fontSize: 28px
    fontWeight: '600'
    lineHeight: '1.3'
    letterSpacing: -0.01em
  h3:
    fontFamily: Manrope
    fontSize: 20px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: 0em
  body-lg:
    fontFamily: Newsreader
    fontSize: 20px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Newsreader
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  label-md:
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1.2'
  caption:
    fontFamily: Manrope
    fontSize: 13px
    fontWeight: '400'
    lineHeight: '1.4'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  container-max: 1280px
  sidebar-width: 280px
  gutter: 2rem
  section-padding: 4rem
  stack-sm: 0.5rem
  stack-md: 1.5rem
  stack-lg: 3rem
---

## Brand & Style
The design system is engineered to support high-density technical information while maintaining the prestige of an academic publication. The brand personality is authoritative, visionary, and intellectually rigorous. It balances the timeless nature of a research paper with the functional clarity of a modern digital interface. 

The aesthetic follows a **Minimalist Corporate** approach. It leverages significant whitespace to reduce cognitive load and focuses on precise typographic hierarchy rather than decorative elements. The goal is to evoke a sense of "digital paper"—an environment where the user feels they are engaging with a definitive source of truth.

## Colors
This design system utilizes a palette rooted in traditional academic values but optimized for digital accessibility. 

- **Primary (Heritage Maroon):** Used for key branding elements, primary call-to-action buttons, and active states in the navigation sidebar. It provides a striking contrast against the neutral backgrounds.
- **Secondary (Midnight Blue):** Employed for headers and UI framing to provide a stable, professional anchor.
- **Tertiary (Paper White):** A slightly warm, off-white used for the main content background to reduce eye strain compared to pure white.
- **Neutral (Ink):** A dark charcoal used for body text to ensure maximum legibility and AA/AAA accessibility compliance.

## Typography
Typography is the cornerstone of this design system. We use a "pairing of opposites" to distinguish between functional UI and narrative content.

**Headlines** utilize **Manrope**, a clean, geometric sans-serif. This choice ensures that section headers and navigation elements feel modern and systematic. 

**Body Text** utilizes **Newsreader**, an authoritative serif font specifically designed for long-form reading on screens. It provides the "academic" weight required for a technical brief. 

For maximum readability, the measure (line length) of body text should be restricted to between 65–75 characters.

## Layout & Spacing
The layout follows a **Fixed Grid** model optimized for documentation. The content is centered within a maximum-width container to prevent line lengths from becoming unwieldy on ultra-wide monitors.

1.  **Sidebar:** A fixed-position navigation sidebar sits on the left (or top on mobile), providing a table of contents. It uses a subtle vertical border rather than a heavy shadow.
2.  **Main Content:** A 12-column grid structure where the main prose occupies the central 8 columns, leaving the remaining 4 for marginalia, callouts, or whitespace.
3.  **Rhythm:** We use an 8px base unit for all spacing. Section headers are separated by "stack-lg" units to provide a clear visual break between technical topics.

## Elevation & Depth
To maintain an academic and clean aesthetic, this design system avoids heavy drop shadows and dramatic depth. Instead, it uses:

- **Tonal Layering:** The primary background is `Tertiary (Paper White)`, while the sidebar or code snippets use a slightly cooler or warmer neutral to create separation.
- **Low-Contrast Outlines:** Interactive elements like callout boxes or input fields use a 1px solid border in a soft grey or a muted version of the primary color.
- **Subtle Surface Lift:** Only high-priority elements (like active modals or primary buttons) use an extremely diffused, low-opacity shadow (#000000 at 5%) to indicate interactability.

## Shapes
The design system uses **Soft (0.25rem)** roundedness. This subtle rounding softens the technical nature of the brief without making it feel overly "consumer-oriented" or "playful." 

- **Cards and Callouts:** Use `rounded-lg` (0.5rem) to distinguish them from the main flow of text.
- **Buttons and Inputs:** Use the base `rounded` (0.25rem) to maintain a sharp, professional appearance.
- **Images/Figures:** Should remain sharp (0px) to mimic traditional publication styles.

## Components
Consistent implementation of components ensures the brief feels like a cohesive document.

### Navigation Sidebar
The sidebar features a nested list of links. The active state is indicated by a bold `Primary Color` left-border (4px) and a subtle weight change in the text. Use `Manrope` for all sidebar labels.

### Section Headers
H1 and H2 headers should always be preceded by ample whitespace. H2 headers include a subtle horizontal rule underneath them, rendered in a 1px light grey, to provide structural anchoring.

### Callout Boxes (Principles)
Key principles are housed in callout boxes. These boxes have a light background (tinted 5% of the primary color), a 1px solid border of the primary color, and a small icon or label in the top left. They use the `Newsreader` font for the content to maintain the narrative flow.

### Buttons
Primary buttons are solid `Primary Color` with white `Manrope` text. Secondary buttons use an outline style. All buttons use a 0.25rem corner radius.

### Technical Lists
Bulleted lists should use custom square markers in the `Secondary Color` to reinforce the modern, geometric aesthetic of the system.