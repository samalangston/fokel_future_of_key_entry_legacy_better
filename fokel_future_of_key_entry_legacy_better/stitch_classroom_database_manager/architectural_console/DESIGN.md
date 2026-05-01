---
name: Architectural Console
colors:
  surface: '#051424'
  surface-dim: '#051424'
  surface-bright: '#2c3a4c'
  surface-container-lowest: '#010f1f'
  surface-container-low: '#0d1c2d'
  surface-container: '#122131'
  surface-container-high: '#1c2b3c'
  surface-container-highest: '#273647'
  on-surface: '#d4e4fa'
  on-surface-variant: '#bdc8d1'
  inverse-surface: '#d4e4fa'
  inverse-on-surface: '#233143'
  outline: '#87929a'
  outline-variant: '#3e484f'
  surface-tint: '#7bd0ff'
  primary: '#8ed5ff'
  on-primary: '#00354a'
  primary-container: '#38bdf8'
  on-primary-container: '#004965'
  inverse-primary: '#00668a'
  secondary: '#bcc7de'
  on-secondary: '#263143'
  secondary-container: '#3e495d'
  on-secondary-container: '#aeb9d0'
  tertiary: '#c5cce6'
  on-tertiary: '#283044'
  tertiary-container: '#a9b1ca'
  on-tertiary-container: '#3c4459'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#c4e7ff'
  primary-fixed-dim: '#7bd0ff'
  on-primary-fixed: '#001e2c'
  on-primary-fixed-variant: '#004c69'
  secondary-fixed: '#d8e3fb'
  secondary-fixed-dim: '#bcc7de'
  on-secondary-fixed: '#111c2d'
  on-secondary-fixed-variant: '#3c475a'
  tertiary-fixed: '#dae2fd'
  tertiary-fixed-dim: '#bec6e0'
  on-tertiary-fixed: '#131b2e'
  on-tertiary-fixed-variant: '#3f465c'
  background: '#051424'
  on-background: '#d4e4fa'
  surface-variant: '#273647'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 30px
    fontWeight: '600'
    lineHeight: 38px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  body-base:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  mono-data:
    fontFamily: monospace
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 16px
  margin: 24px
  container-max: 1440px
---

## Brand & Style

This design system is built upon the principles of **Architectural Precision** and **Systemic Reliability**. Designed specifically for high-density database management environments, the aesthetic favors utility over decoration. The style is a blend of **Minimalism** and **Modern Corporate**, utilizing a restrained palette to reduce cognitive load while maintaining a sophisticated "tech" atmosphere.

The UI should evoke a sense of absolute stability—essential for users managing mission-critical data. Every element is aligned to a strict logical grid, ensuring that the interface feels engineered rather than merely decorated. Whitespace is used strategically to separate complex data clusters, and interactions are designed to be snappy and predictable.

## Colors

The palette is anchored in a dark-mode-first approach to reduce eye strain during long technical sessions. The foundation consists of **Deep Blues** (for depth and branding) and **Slate Grays** (for structural elements and secondary text).

- **Primary (#38BDF8):** An electric sky blue used sparingly for primary actions, progress indicators, and active states. It provides high contrast against the dark backgrounds.
- **Secondary (#1E293B):** A muted slate blue used for surface elements like cards, navigation sidebars, and header backgrounds.
- **Tertiary (#0F172A):** The "True Deep" blue-black used for the primary application canvas.
- **Neutral (#94A3B8):** A balanced slate gray used for body text, borders, and icons to maintain a professional, low-vibrancy environment.
- **Success/Error:** Use emerald for positive confirmations and rose for destructive actions, but always in desaturated tones to match the "tech" feel.

## Typography

The design system utilizes **Inter** for all UI elements. Inter was selected for its exceptional legibility in technical contexts, specifically its tall x-height and distinct character shapes which prevent "character blurring" in high-density data tables.

- **Headlines:** Use a semi-bold weight with slight negative letter spacing to feel "tight" and authoritative.
- **Body Text:** The standard is 14px for general interface text. For data-heavy tables, 13px is acceptable to increase information density without sacrificing clarity.
- **Labels:** Small, uppercase labels are used for metadata and section headers within sidebars to create a clear visual hierarchy.
- **Data Display:** For actual database values (strings, integers, IDs), fallback to a system monospaced font to ensure alignment and readability.

## Layout & Spacing

This design system employs a **Fluid Grid** model with a strict 4px baseline rhythm. All margins, paddings, and component heights must be multiples of 4px.

- **Grid:** Use a 12-column layout for dashboards and complex form views.
- **Gutters:** A standard 16px (4 units) gutter provides enough breathing room for data-heavy rows.
- **Density:** The system supports "Standard" and "Compact" views. In Compact view, vertical padding is reduced by 50% to allow more rows of data to be visible above the fold.
- **Alignment:** Navigation is consistently pinned to the left (240px width), with the main content area expanding to fill the remaining viewport.

## Elevation & Depth

Visual hierarchy is established through **Tonal Layers** rather than heavy shadows. In a dark technical environment, light is treated as a subtle indicator of "height."

1. **Base Layer (Level 0):** The primary background (#0F172A).
2. **Surface Layer (Level 1):** Cards, sidebars, and tables use a slightly lighter slate (#1E293B). 
3. **Overlay Layer (Level 2):** Modals and dropdowns use an even lighter tint with a **Low-contrast outline** (1px solid #334155) to define edges against the background.
4. **Shadows:** Only used for floating elements (modals). Shadows should be sharp, dark, and highly diffused (e.g., `0 10px 15px -3px rgba(0, 0, 0, 0.5)`).

## Shapes

The shape language is **Soft (0.25rem)**. This subtle rounding removes the aggressive sharpness of a purely brutalist UI while maintaining a professional, structured "box" feel. 

- **Standard Elements:** Buttons, inputs, and small cards use a 4px radius.
- **Large Containers:** Main content panels or large modals may use a 8px (rounded-lg) radius to feel more "contained."
- **Badges:** Selection badges and status indicators use a 4px radius; avoid pill-shapes to maintain the architectural, rectangular theme.

## Components

### Action Buttons
- **Primary:** Solid sky blue (#38BDF8) with dark navy text. No gradients. Hover state is a subtle brightness increase.
- **Secondary:** Ghost style with a 1px border of #334155 and light gray text. High contrast on hover.
- **Danger:** Desaturated red background with white text, reserved for "Drop Table" or "Delete" actions.

### Form Inputs
- **Base State:** Dark background (#0F172A) with a 1px slate border (#334155). 
- **Focus State:** Border changes to primary sky blue with a subtle 2px outer glow (ring).
- **Labeling:** Labels sit above the input in a smaller, medium-weight font.

### User Selection Badges (Chips)
- Used for filtering or multi-select roles.
- Styled with a subtle slate fill (#334155) and a 1px border. 
- Include a "close" icon (X) that appears on hover for easy removal.

### Data Tables
- Header rows should have a slightly darker background than body rows.
- Use horizontal dividers only (1px #1E293B). Avoid vertical lines to keep the view clean.
- Row hover states should use a subtle highlight color (#1E293B).

### Status Indicators
- Small, solid circles (8px) paired with text. 
- Colors: Green (Connected), Amber (Syncing), Red (Disconnected), Gray (Idle).