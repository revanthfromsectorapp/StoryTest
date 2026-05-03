# 🟠 Crunchyroll Mobile App Design System
> **Version:** 2.0.0 (July 2024 Refresh)  
> **Identity:** High-contrast, immersive anime streaming experience.
---
## 🎨 Color Palette
| Token | Hex | Preview | Use Case |
| :--- | :--- | :--- | :--- |
| `primary` | `#F47521` | 🟠 | Signature Orange (CTAs, Play Buttons) |
| `primary-active` | `#CB5A16` | 🟤 | Pressed/Active state for Orange elements |
| `canvas` | `#000000` | ⚫ | Pure Black (OLED Backgrounds) |
| `surface-soft` | `#141414` | 🌑 | Card backgrounds & Section dividers |
| `surface-strong`| `#1F1F1F` | 🌑 | Elevated surfaces (Modals, Overlays) |
| `ink` | `#FFFFFF` | ⚪ | Primary text & Headlines |
| `body` | `#E5E5E5` | ⚪ | Paragraphs & Summaries |
| `muted` | `#8C8C8C` | 🔘 | Metadata (Year, Episodes, Genre) |
| `accent-taupe` | `#B8B0A5` | 🟤 | Secondary tags & Manga textures |
---
## typography Hierarchy
**Primary Font:** `Crunchyroll Atyp` (Custom)  
**Secondary Font:** `Roboto` (System Fallback)
| Token | Size | Weight | Line Height | Usage |
| :--- | :--- | :--- | :--- | :--- |
| `display-xl` | `34px` | `800` | `1.1` | Hero Series Titles |
| `display-lg` | `24px` | `700` | `1.2` | Section Headlines |
| `title-md` | `18px` | `600` | `1.4` | Card Titles / Show Names |
| `body-md` | `14px` | `400` | `1.5` | Plot Summaries |
| `caption` | `12px` | `500` | `1.2` | Metadata & Tags |
| `button` | `14px` | `700` | `1.0` | CTA Labels (Uppercase) |
---
## 📐 Layout & Spacing
| Token | Value | Use Case |
| :--- | :--- | :--- |
| `spacing-xs` | `4px` | Micro-adjustments |
| `spacing-sm` | `8px` | Internal card padding |
| `spacing-md` | `12px` | Gutter between cards |
| `spacing-lg` | `16px` | Page margins |
| `spacing-section`| `32px` | Vertical gap between categories |
| **Grid** | `4-Column` | Mobile standard with 16px margins |
---
## 🧩 Core Components
### 🖱️ Buttons
*   **`button-primary`**: 
    *   **Style**: Background `{colors.primary}`, Text `{colors.canvas}`
    *   **Shape**: `{rounded.md}` (8px)
    *   **Behavior**: High voltage, used for "Watch Now" and "Subscribe".
### 🖼️ Content Cards
*   **`content-card`**: 
    *   **Aspect Ratio**: `2:3` (Poster Layout)
    *   **Radius**: `{rounded.md}` (8px)
    *   **Detail**: Features a subtle progress bar in `{colors.primary}` at the bottom for "In-progress" shows.
### 🧭 Navigation
*   **`tab-bar`**: 
    *   **Blur**: 95% opacity `{colors.canvas}` with a `{colors.hairline}` top border.
    *   **Icons**: High-contrast white glyphs, turning orange when active.
---
## 💡 Design Principles
1.  **Immersive "Dark Room" Logic**: The UI remains invisible (Pure Black) to let the vibrant anime artwork be the sole focus.
2.  **Action Voltage**: The signature Orange is reserved *strictly* for interactive triggers to avoid cognitive overload.
3.  **Content Density**: Uses a tight grid to maximize show discoverability while maintaining clear metadata hierarchy.
---
## 📱 Responsive & Motion
*   **Adaptive Grids**: 2-up cards on small devices, 3-up on larger smartphones.
*   **Motion**: 
    *   **Taps**: Subtle spring scale-down (0.98x).
    *   **Transitions**: Horizontal slides for sub-menus; Vertical slides for full-screen player.
*   **Loading**: Shimmer skeleton screens using `{colors.surface-soft}`.
