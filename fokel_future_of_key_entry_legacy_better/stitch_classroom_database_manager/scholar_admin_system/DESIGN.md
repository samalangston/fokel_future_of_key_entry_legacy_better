---
name: Scholar Admin System
colors:
  surface: '#f8f9ff'
  surface-dim: '#cbdbf5'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e5eeff'
  surface-container-high: '#dce9ff'
  surface-container-highest: '#d3e4fe'
  on-surface: '#0b1c30'
  on-surface-variant: '#434651'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#747782'
  outline-variant: '#c4c6d3'
  surface-tint: '#375ca8'
  primary: '#002155'
  on-primary: '#ffffff'
  primary-container: '#003580'
  on-primary-container: '#7fa1f2'
  inverse-primary: '#b0c6ff'
  secondary: '#4b5a9c'
  on-secondary: '#ffffff'
  secondary-container: '#a6b5fd'
  on-secondary-container: '#354585'
  tertiary: '#002a1a'
  on-tertiary: '#ffffff'
  tertiary-container: '#00422b'
  on-tertiary-container: '#10b981'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d9e2ff'
  primary-fixed-dim: '#b0c6ff'
  on-primary-fixed: '#001945'
  on-primary-fixed-variant: '#1a438e'
  secondary-fixed: '#dde1ff'
  secondary-fixed-dim: '#b8c4ff'
  on-secondary-fixed: '#001354'
  on-secondary-fixed-variant: '#334282'
  tertiary-fixed: '#6ffbbe'
  tertiary-fixed-dim: '#4edea3'
  on-tertiary-fixed: '#002113'
  on-tertiary-fixed-variant: '#005236'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: '1.4'
  body-base:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
  data-tabular:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '500'
    lineHeight: '1.5'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  sidebar-width: 240px
  container-padding: 2rem
  stack-gap: 1.5rem
  grid-gutter: 1rem
  element-padding-sm: 0.75rem
  element-padding-md: 1.25rem
---

## Brand & Style

The brand personality is academic, authoritative, and clinical. It is designed for high-stakes administrative environments where data clarity and system reliability are paramount. The aesthetic favors a "Scholar Admin" look: a refined take on the traditional enterprise dashboard that prioritizes information density without sacrificing visual breathing room.

The design style is **Corporate / Modern**. It utilizes a systematic approach to layout, a restrained color palette, and clear visual hierarchies. The interface communicates trust and precision through structured grids, subtle tonal layering, and high-contrast typography, ensuring that complex database and permission structures remain legible at a glance.

## Colors

The color palette is anchored by a deep "Scholar Blue" used for primary actions and branding, evoking a sense of institutional stability. 

- **Primary:** A deep, professional blue used for the logo, primary call-to-action buttons, and active navigation icons.
- **Secondary:** A soft, muted indigo/periwinkle used for secondary actions and subtle highlights, providing contrast against the primary blue without being aggressive.
- **Success/Status:** A vibrant emerald green is reserved strictly for "Online" or "Active" status indicators to provide immediate visual feedback.
- **Neutrals:** The system uses a range of slate grays. The background is a very pale cool-gray to reduce eye strain, while the sidebar uses a slightly more saturated tint to define the primary navigation zone.

## Typography

This design system utilizes **Inter** across all levels to leverage its exceptional readability in data-heavy environments. 

The typography strategy focuses on a clear "Scale of Importance." Large, bold displays are used for page titles to ground the user, while smaller, semi-bold caps are used for category labels and table headers to maximize vertical space. Data points (like version numbers or latency) use a medium weight to stand out against standard body text. Line heights are kept tight but comfortable to maintain the "Scholar" focus on information density.

## Layout & Spacing

The layout utilizes a **Fixed Sidebar + Fluid Content** model. The sidebar is a persistent navigation anchor, while the main content area expands to accommodate complex data tables and management cards.

A strict 8px spacing rhythm is applied. Sections are separated by 24px or 32px of vertical space to group related information. Inside components like cards, a 16px (1rem) or 20px padding is standard to ensure the interface feels dense and professional, allowing for multiple modules to be visible on a single screen without scrolling. Content within cards is typically organized in a two-column or multi-column grid depending on the data type.

## Elevation & Depth

Visual hierarchy is established primarily through **Tonal Layers** and **Low-Contrast Outlines** rather than aggressive shadows.

1.  **Level 0 (Base):** The main background uses a soft, cool-gray tint (`#F8FAFC`).
2.  **Level 1 (Sidebar):** The sidebar uses a subtle tint difference to separate it from the main workspace.
3.  **Level 2 (Cards/Modules):** Functional units are placed on pure white surfaces. These surfaces are defined by a very light 1px border or an extremely diffused, low-opacity shadow to provide just enough lift to signify interactability.
4.  **Level 3 (Interactive Overlays):** Modals or tooltips use a slightly more pronounced shadow with a wider blur radius to indicate they sit atop the administrative grid.

## Shapes

The shape language is defined by **Soft** (0.25rem) roundedness. This minimal radius maintains a serious, "grid-like" institutional feel while removing the harshness of sharp 90-degree corners.

- **Buttons & Inputs:** Use a standard 4px (0.25rem) radius.
- **Data Cards:** Use a slightly larger 8px (0.5rem) radius to soften the larger surface areas.
- **Status Tags:** Use a pill-shape or a 4px radius depending on the visual weight required for the tag.
- **Icons:** Enclosed within rounded-square containers to mirror the card shapes.

## Components

### Buttons
- **Primary:** Solid deep blue with white text. High contrast for the most important system actions.
- **Secondary/Action:** Ghost buttons or light blue backgrounds with primary-colored text for auxiliary actions like "Export" or "Add."
- **Sidebar Items:** Clean labels with subtle icons. The "Active" state uses a white background block to create a "tab" effect against the tinted sidebar.

### Cards & Modules
Cards are the primary container for data. They feature a clear header (often with an icon), a central data body, and a footer for metadata like "Latency" or "Storage." Active modules may feature a colored top-border or status indicator.

### Inputs & Tables
- **Text Inputs:** Low-profile borders that darken on focus. 
- **Data Tables:** High-density rows with light horizontal dividers. The header row should be visually distinct using a light gray background and all-caps labels.
- **Status Indicators:** Small colored dots paired with text (e.g., "• ONLINE") to provide immediate state awareness.

### Navigation
Global navigation is split between a top-bar for system-level context (Audit, Security) and a vertical sidebar for localized toolsets (Databases, Permissions).