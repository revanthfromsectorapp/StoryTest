---
version: 1.0.0
name: [Project Name]
description: [Short high-level description of the aesthetic. E.g., "A dark, glassmorphic productivity interface focused on high-contrast typography and neon accent voltages."]

colors:
  # Brand & Primary Actions
  primary: "#[Hex Code]"        # The main brand color (CTAs, Links)
  primary-active: "#[Hex]"     # Pressed state
  primary-disabled: "#[Hex]"   # Inactive state
  
  # Backgrounds & Surfaces
  canvas: "#[Hex]"             # Main page background
  surface-soft: "#[Hex]"       # Secondary backgrounds (Cards, Sections)
  surface-strong: "#[Hex]"     # Elevated backgrounds (Modals, Popups)
  
  # Text & Ink
  ink: "#[Hex]"                # Primary text color (Headlines)
  body: "#[Hex]"               # Secondary text (Paragraphs)
  muted: "#[Hex]"              # De-emphasized text (Captions, Footers)
  
  # Decorative & Semantic
  hairline: "#[Hex]"           # 1px borders and dividers
  accent: "#[Hex]"             # Neon or highlight colors
  error: "#[Hex]"              # Validation/Error states
  success: "#[Hex]"            # Success/Confirmation

typography:
  display-xl:
    fontFamily: "[Font Name], sans-serif"
    fontSize: "48px"
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: "-0.02em"
  display-lg:
    fontFamily: "[Font Name], sans-serif"
    fontSize: "32px"
    fontWeight: 600
    lineHeight: 1.2
  title-md:
    fontFamily: "[Font Name], sans-serif"
    fontSize: "20px"
    fontWeight: 500
    lineHeight: 1.4
  body-md:
    fontFamily: "[Secondary Font], sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.6
  caption:
    fontFamily: "[Secondary Font], sans-serif"
    fontSize: "13px"
    fontWeight: 500
    lineHeight: 1.2
  button:
    fontFamily: "[Font Name], sans-serif"
    fontSize: "14px"
    fontWeight: 600
    lineHeight: 1.0

rounded:
  none: "0px"
  sm: "4px"
  md: "8px"
  lg: "16px"
  xl: "24px"
  full: "9999px"

spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "48px"
  section: "96px"

components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.canvas}"
    typography: "{typography.button}"
    rounded: "{rounded.md}"
    padding: "12px 24px"
    height: "48px"
  card-base:
    backgroundColor: "{colors.surface-soft}"
    border: "1px solid {colors.hairline}"
    rounded: "{rounded.lg}"
    padding: "{spacing.lg}"
  nav-bar:
    backgroundColor: "rgba(255, 255, 255, 0.8)" # Blur/Opacity support
    height: "72px"
    borderBottom: "1px solid {colors.hairline}"
---

## 1. Design Principles & Overview
*   **Aesthetic Identity**: Describe the "vibe" (e.g., "Minimalist Industrial," "Vibrant Consumer," "Cyberpunk Dark").
*   **Core Strategy**: How does the design handle hierarchy? (e.g., "Photography-led" or "Type-heavy").
*   **Key Characteristics**: List 3-5 unique traits (e.g., "Heavy use of backdrop blurs," "No sharp corners," "Single accent color policy").

## 2. Layout & Spacing
*   **Grid System**: Define columns (e.g., 12-column desktop grid with 24px gutters).
*   **Container Width**: Max-width for content (e.g., 1280px).
*   **Whitespace Philosophy**: How much breathing room is between sections? (e.g., "Generous vertical padding of 96px for editorial impact").

## 3. Elevation & Depth
*   **Shadow Tiers**: Define your `box-shadow` values (e.g., Soft: `0 4px 12px rgba(0,0,0,0.05)`, Strong: `0 12px 32px rgba(0,0,0,0.15)`).
*   **Surface Separation**: How do elements layer? (e.g., "Cards use a 1px border instead of shadows to maintain a flat look").

## 4. Key Components
*   **Navigation**: How the menu behaves (Sticky vs. Fixed, Mobile Hamburger logic).
*   **Hero Section**: Structure of the landing fold (Headline size, CTA placement).
*   **Inputs & Forms**: Hover states, focus rings, and error message styling.

## 5. Responsive Behavior
*   **Breakpoints**: Mobile (< 768px), Tablet (768px - 1024px), Desktop (> 1024px).
*   **Adaptation Strategy**: E.g., "Cards stack vertically on mobile; navigation collapses into a bottom-sheet drawer."

## 6. Implementation Notes
*   **Interactions**: Transition speeds (e.g., `ease-in-out 0.2s`).
*   **Empty States**: How lists look when empty.
*   **Loading States**: Shimmer effect vs. Spinner style.
