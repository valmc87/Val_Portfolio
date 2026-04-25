---
name: stretch-dark-mode
description: Add a dark mode toggle to an existing personal branding website. Use as a stretch goal after the base site is built. Pure CSS + minimal JS.
---

# Stretch Goal: Dark Mode Toggle 🌙

Add a dark/light mode toggle to the existing personal branding website.

## What to Do

1. Read the existing `index.html` and `style.css`
2. Add a toggle button (sun/moon icon) fixed in the top-right corner
3. Add CSS custom properties (variables) for all colors
4. Add minimal JavaScript to toggle a `dark-mode` class on `<body>` and save preference to localStorage

## Implementation

### CSS Changes (in `style.css`)
- Define color variables on `:root` for light mode (backgrounds, text, accents, card colors)
- Define overrides on `body.dark-mode` that swap to dark equivalents
- Replace all hardcoded colors in existing CSS with the variables
- Style the toggle button to be subtle but visible in both modes

### HTML Changes (in `index.html`)
- Add a toggle button in the header area: a small circular button with 🌙 / ☀️
- Add a small `<script>` at the bottom of `<body>` that:
  - Toggles `dark-mode` class on body when clicked
  - Saves preference to `localStorage`
  - Loads saved preference on page load

### Dark Mode Colors
- Background: dark gray (#1a1a2e or #0d1117)
- Text: light gray (#e0e0e0 or #f0f0f0)
- Cards/sections: slightly lighter dark (#16213e or #161b22)
- Accent colors: keep the existing accents but adjust brightness if needed for contrast
- Links: brighten slightly for visibility

## Constraints
- Keep the JavaScript minimal (under 15 lines)
- Preserve the existing theme's personality — dark mode should feel like the same site, just inverted
- Ensure sufficient contrast in both modes (WCAG AA)
- Toggle should be visible and accessible in both modes
