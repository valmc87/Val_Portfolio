---
name: stretch-animations
description: Add CSS animations and hover effects to an existing personal branding website. Use as a stretch goal after the base site is built. Pure CSS only.
---

# Stretch Goal: CSS Animations ✨

Add smooth animations and hover effects to the existing personal branding website.

## What to Do

1. Read the existing `index.html` and `style.css`
2. Add CSS animations — no JavaScript required

## Animations to Add

### Entrance Animations
- **Fade-in on load:** Sections fade in with a slight upward slide when the page loads. Use `@keyframes` with `opacity` and `transform: translateY`.
- **Staggered timing:** Each section animates slightly after the previous one using `animation-delay`.

### Hover Effects
- **Cards:** Gentle lift (translateY -5px) + shadow increase on hover
- **Skills/tags:** Scale up slightly (1.05) + color shift on hover
- **Social links:** Scale up (1.15) + rotate slightly on hover
- **Profile photo:** Subtle scale (1.03) on hover

### Subtle Continuous Animations
- **Hero section:** A gentle gradient animation on the background (if gradient exists) — slowly shifting colors
- **Or:** A subtle floating animation on the profile photo (translateY up and down, 3s loop)

## Implementation

Add all animations in `style.css`. Use:
- `@keyframes` for custom animations
- `transition` for hover effects (0.3s ease)
- `animation` shorthand for entrance and continuous animations
- `animation-fill-mode: both` to keep final state

## Constraints
- **Pure CSS only.** No JavaScript, no animation libraries.
- **Subtle and tasteful.** Animations should enhance, not distract. Keep durations short (0.3–0.6s for transitions, 0.5–1s for entrances).
- **Respect `prefers-reduced-motion`.** Add a media query that disables animations for users who prefer reduced motion.
- **Don't break the layout.** Animations should not cause content shifts or overflow issues.
