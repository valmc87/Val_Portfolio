---
name: stretch-visitor-counter
description: Add a visitor counter badge to an existing personal branding website. Uses a free external badge service. No backend needed.
---

# Stretch Goal: Visitor Counter 👀

Add a visitor counter to the existing personal branding website using a free badge service.

## What to Do

1. Read the existing `index.html`
2. Add a visitor counter badge to the footer area
3. No backend or JavaScript needed — uses an external image badge service

## Implementation

### Using hits.sh (free, no signup)

Add this image tag to the footer section of `index.html`:

```html
<img src="https://hits.sh/USERNAME.github.io.svg?style=flat-square&label=visitors&color=6C63FF" alt="Visitor count">
```

Replace `USERNAME` with the attendee's actual GitHub username.

### Styling
- Place the badge in the footer, centered or aligned with other footer content
- Optionally wrap it in a small container with some padding
- The badge color can be customized via the `color` parameter in the URL (use hex without #)

### Alternative: shields.io with a custom label

```html
<img src="https://img.shields.io/badge/visitors-welcome-brightgreen?style=flat-square" alt="Visitors welcome">
```

This is a static badge (doesn't count) but looks nice. Use hits.sh for actual counting.

## Constraints
- **No JavaScript required** — it's just an `<img>` tag
- **No signup required** — hits.sh works automatically
- **Privacy-friendly** — only counts page loads, no tracking
- **The counter resets if the URL changes** — make sure the URL matches the actual GitHub Pages URL
