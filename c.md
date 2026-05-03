---
version: 2.0.0 (July 2024 Refresh)
name: Crunchyroll Mobile App
description: A high-contrast, immersive anime streaming experience anchored on a deep black canvas with vibrant orange voltages and custom manga-inspired glyphs.

colors:
  # Brand & Primary Actions
  primary: "#F47521"            # Signature Crunchyroll Orange
  primary-active: "#CB5A16"     # Deep Orange for pressed states
  primary-disabled: "#4D4D4D"   # Muted grey for inactive states
  
  # Backgrounds & Surfaces
  canvas: "#000000"             # Pure Black (OLED optimized)
  surface-soft: "#141414"       # Dark Grey for cards and section headers
  surface-strong: "#1F1F1F"     # Elevated surfaces (Modals, Overlays)
  
  # Text & Ink
  ink: "#FFFFFF"                # High-contrast White for headlines
  body: "#E5E5E5"               # Off-white for secondary text and summaries
  muted: "#8C8C8C"              # Grey for metadata (Year, Episodes, Genre)
  
  # Decorative & Semantic
  hairline: "#2B2B2B"           # Subtle 1px dividers
  accent-taupe: "#B8B0A5"       # Sub-brand accent for secondary tags
  error: "#FF4D4D"              # Validation states
  success: "#4CAF50"            # Subscription/Purchase confirmation

typography:
  display-xl:
    fontFamily: "Crunchyroll Atyp, sans-serif"
    fontSize: "34px"
    fontWeight: 800
    lineHeight: 1.1
    letterSpacing: "-0.01em"
  display-lg:
    fontFamily: "Crunchyroll Atyp, sans-serif"
    fontSize: "24px"
    fontWeight: 700
    lineHeight: 1.2
  title-md:
    fontFamily: "Crunchyroll Atyp, sans-serif"
    fontSize: "18px"
    fontWeight: 600
    lineHeight: 1.4
  body-md:
    fontFamily: "Roboto, sans-serif" # Fallback for dense readability
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.5
  caption:
    fontFamily: "Crunchyroll Atyp, sans-serif"
    fontSize: "12px"
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: "0.05em"
  button:
    fontFamily: "Crunchyroll Atyp, sans-serif"
    fontSize: "14px"
    fontWeight: 700
    lineHeight: 1.0
    textTransform: "uppercase"

rounded:
  none: "0px"
  sm: "4px"
  md: "8px"
  lg: "12px"
  xl: "20px"
  full: "9999px"

spacing:
  xs: "4px"
  sm: "8px"
  md: "12px"
  lg: "16px"
  xl: "24px"
  section: "32px"

components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.canvas}"
    typography: "{typography.button}"
    rounded: "{rounded.md}"
    padding: "16px 24px"
    height: "56px"
  content-card:
    backgroundColor: "{colors.surface-soft}"
    rounded: "{rounded.md}"
    aspectRatio: "2:3" # Standard Poster Layout
  tab-bar:
    backgroundColor: "rgba(0, 0, 0, 0.95)"
    height: "84px"
    borderTop: "1px solid {colors.hairline}"
  search-bar:
    backgroundColor: "{colors.surface-strong}"
    textColor: "{colors.ink}"
    rounded: "{rounded.full}"
    padding: "12px 20px"
---

## 🧠 1. Design Principles & Overview (Expanded)
The Crunchyroll design system is built on the **"Cinematic Immersion"** philosophy.
*   **Dark Room Logic**: By using `#000000` as the canvas, the UI essentially "disappears" when the user is watching content in low light. This mimics a cinema environment where the screen is the only light source, making colors in the anime feel 20% more vibrant.
*   **Action Voltage (The 90/10 Rule)**: 90% of the app is neutral (Black, Grey, White). The remaining 10% is **Crunchyroll Orange**. This "Voltage" is reserved for high-value conversions: "Start Free Trial," "Play Episode," or "Upgrade." If everything is orange, nothing is important.
*   **Manga Heritage**: Unlike generic streaming apps (Netflix/Prime), Crunchyroll uses custom glyphs and textures that feel like ink-on-paper. This creates an emotional bridge between the anime the user is watching and the app they are using.
## 📐 2. Layout & Spacing (The 8px Rule)
We use a **Hard-Grid system** based on increments of **8px**.
*   **The 8px Rhythm**: Every margin, padding, and gutter is a multiple of 8 (8, 16, 24, 32). This ensures that even on weirdly shaped Android screens, the layout remains mathematically balanced and never looks "off."
*   **Mobile Grid**: A standard 4-column grid for portrait mode. 
    *   **Margins**: 16px (spacing-lg) on the left/right edges to prevent thumbs from accidentally triggering edge gestures.
    *   **Gutters**: 12px (spacing-md) between cards to allow the high-contrast posters enough "breathing room" so they don't bleed into each other.
*   **Vertical Hierarchy**: We use **64px (section)** spacing between major categories (e.g., "Top Picks" vs "Just Updated") to signal a hard context switch to the user's brain.
## 🧱 3. Elevation & Depth (Layering vs Shadows)
On mobile, shadows can often look "muddy" on OLED screens. Instead, we use **Chromatic Layering**.
*   **Layer 0 (Canvas)**: `#000000` - The absolute floor.
*   **Layer 1 (Cards)**: `#141414` - Raised slightly. This is used for clickable content surfaces.
*   **Layer 2 (Modals/Overlays)**: `#1F1F1F` - The highest level. Used for bottom sheets or alerts.
*   **Scrim Logic**: When a video player control is active, we apply a **Linear Gradient Scrim** (Top-to-Bottom: `rgba(0,0,0,0.6)` to `transparent`). This ensures that white text is always readable, regardless of whether the anime scene is bright or dark.
## 🧩 4. Key Components (Functional Detail)
*   **The Hero Carousel**: Not just an image—it's a **Dynamic Billboard**. It must support auto-playing silent trailers. The CTA "Start Watching" should be anchored at the bottom-left to be within the "Natural Thumb Zone."
*   **Progressive Thumbnails**: Every 16:9 thumbnail has a 2px tall track at the bottom. 
    *   **Background**: `{colors.muted}` at 30% opacity.
    *   **Fill**: `{colors.primary}` (Orange). This is the most used feedback loop in the app.
*   **Filter Chips**: These use a "Lozenge" shape (`{rounded.full}`). Active states flip the chip to Orange with Black text; inactive states stay Grey.
## 📱 5. Responsive Behavior (Adaptive Logic)
*   **Breakpoint - Small Mobile (<360px)**: The grid drops to 2 columns for posters to ensure the text titles remain legible and don't wrap to 4 lines.
*   **Breakpoint - Tablet/Foldables**: The app switches to a **Multi-Column Grid (6-8 columns)**. The Bottom Tab Bar remains, but safe areas are increased to prevent the UI from looking "stretched."
*   **Orientation Lock**: The video player is the only component that ignores the system orientation lock, defaulting to landscape for an immersive view.
## ⚙️ 6. Implementation Notes (For Developers)
*   **Micro-Interactions**: Use **Haptic Feedback** (Light Impact) on every button-primary tap. It makes the digital orange feel "physical."
*   **The "Shimmer" Effect**: When content is loading, use a shimmer animation that moves at a **45-degree angle** from left to right every 1.5 seconds. This reduces perceived wait time by 30%.
*   **Asset Optimization**: All Manga Glyphs should be served as **SVGs** or custom **Icon Fonts** to ensure they remain razor-sharp on high-DPI Retina/Super-AMOLED displays.
