---
name: stretch-favicon
description: Add a favicon to an existing personal branding website. Use as a stretch goal. Generates an SVG favicon from the person's initials.
---

# Stretch Goal: Favicon ⭐

Add a custom favicon to the existing personal branding website.

## What to Do

1. Read the existing `index.html` to get the person's name
2. Generate an SVG favicon using their initials
3. Add the favicon link to `index.html`

## Implementation

### Generate the Favicon
Create a file `favicon.svg` in the project root:
- A rounded square or circle shape
- Background: use the site's primary accent color (read from `style.css`)
- Text: the person's initials (first letter of first + last name) in white, bold, centered
- Keep it simple — SVG favicons work in all modern browsers

### Example SVG
```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100">
  <rect width="100" height="100" rx="20" fill="#6C63FF"/>
  <text x="50" y="55" font-family="Arial,sans-serif" font-size="45" font-weight="bold" fill="white" text-anchor="middle" dominant-baseline="middle">JD</text>
</svg>
```

### Add to HTML
Add this line inside `<head>` in `index.html`:
```html
<link rel="icon" type="image/svg+xml" href="favicon.svg">
```

## Constraints
- **SVG format** — works in all modern browsers, scales perfectly, tiny file size
- **Match the site's theme** — use the accent color from the existing stylesheet
- **No external tools needed** — just an SVG file
