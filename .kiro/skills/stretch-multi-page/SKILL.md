---
name: stretch-multi-page
description: Convert a single-page personal branding website into a multi-page site. Use as a stretch goal after the base site is built.
---

# Stretch Goal: Multi-Page Site 📄

Convert the single-page website into a multi-page site with navigation.

## What to Do

1. Read the existing `index.html` and `style.css`
2. Split sections into separate pages
3. Add a navigation bar that links between pages
4. Keep consistent header/footer across all pages

## Page Structure

### `index.html` (Home)
- Hero/header with name, tagline, photo
- About Me section
- Navigation to other pages

### `skills.html`
- Skills & Passions section (from the original page)
- Achievements section

### `experience.html`
- Experience / Education section
- Could include a timeline layout

### `fun.html`
- Fun Facts section
- Social Links section

## Navigation Bar

Add a `<nav>` element to every page:
- Links: Home | Skills | Experience | Fun
- Highlight the current/active page
- Responsive: horizontal on desktop, hamburger or stacked on mobile (CSS-only if possible)
- Sticky or fixed at the top

## Implementation

1. Create the new HTML files, each with the same `<head>` (linking to `style.css` and Google Fonts)
2. Move the relevant sections from `index.html` into each new page
3. Add the navigation bar to every page
4. Add nav styles to `style.css`
5. Ensure the footer appears on every page

## Constraints
- **HTML + CSS only.** A CSS-only mobile menu is preferred, but a tiny bit of JS for a hamburger toggle is acceptable.
- **Consistent styling.** All pages share the same `style.css`.
- **Working links.** All navigation links must work correctly.
- **Each page stands alone.** Every page has full `<html>`, `<head>`, `<body>` structure.
