---
name: theme-creative-artsy
description: Generate a creative and artsy personal branding website. Use when the attendee wants gradients, unique layouts, and artistic flair. Reads my-profile.md for content.
---

# Theme: Creative & Artsy 🎭

Generate a single-page personal branding website with a **creative, artsy, and visually striking** style.

## Content Source

Read `my-profile.md` in the project root for all personal content (name, tagline, bio, skills, experience, achievements, fun facts, social links, and profile photo filename).

## Files to Generate

1. `index.html` — the complete single-page website
2. `style.css` — all styles in a separate stylesheet

## Visual Style Requirements

- **Color palette:** Rich and dramatic — deep purples, midnight blues, warm golds, or sunset gradients. Use bold color combinations that feel artistic.
- **Gradients:** Use CSS gradients liberally — backgrounds, text overlays, borders. Mix 2–3 colors per gradient.
- **Shapes:** Mix of geometric and organic. Asymmetric layouts welcome. Use CSS clip-path for creative shapes on images or sections.
- **Fonts:** Use Google Fonts — an expressive heading font (e.g., Playfair Display, Abril Fatface, Cormorant Garamond, Space Grotesk) and a complementary body font.
- **Layout:** Break the grid. Use asymmetric layouts, overlapping elements (CSS grid with negative margins or overlap), and varied section widths.
- **Background:** Dark or gradient backgrounds for some sections, light for others. Create visual rhythm through contrast.
- **Hover effects:** Creative transforms — slight rotation, scale, color shift, or shadow changes.
- **Overall feel:** Like a digital art portfolio. Bold, expressive, memorable.

## Section Structure

Build these sections in order, using content from `my-profile.md`:

### 1. Hero / Header
- Dramatic full-width header with gradient background
- Name in large, expressive typography — could use CSS text effects (gradient text, text-shadow)
- Tagline with artistic styling
- Profile photo with creative framing — clip-path shape, gradient border, or artistic overlay (if photo exists in `images/` folder, use it; otherwise generate an SVG placeholder with the person's initials on a dramatic gradient background)

### 2. About Me
- Styled with a pull-quote or magazine-style layout
- Could use a large decorative first letter (drop cap via CSS)
- Contrasting background section

### 3. Skills & Passions
- Creative visualization — could be scattered/cloud-like layout, hexagonal tiles, or overlapping cards
- Each skill has visual personality

### 4. Experience / Education
- Vertical timeline with artistic connectors (gradient lines, dots, or custom shapes)
- Each entry is a styled card with subtle asymmetry

### 5. Achievements
- Gallery-style or masonry-like grid
- Each achievement in a visually distinct card with gradient accents

### 6. Fun Facts
- The most creative section — could be a collage layout, polaroid-style cards, or an artistic grid
- Each fact gets unique visual treatment

### 7. Social Links
- Artistic icon buttons with gradient backgrounds or creative shapes
- Use inline SVG icons or Unicode symbols
- Hover: dramatic transform or color shift

### 8. Footer
- Artistic footer with gradient background
- "Built with 🎭 and AI at Women In Tech Workshop"
- Include #GivetoGain

## Technical Requirements

- **Pure HTML + CSS only.** No JavaScript. No frameworks. No build tools.
- **Mobile responsive.** Must look good on phones (use CSS flexbox/grid, media queries). Simplify the creative layouts for mobile.
- **Single page.** Everything in one `index.html`.
- **External stylesheet.** All CSS in `style.css`, linked from `index.html`.
- **Google Fonts.** Import via `<link>` tag in HTML head.
- **No external dependencies** other than Google Fonts.
- **Semantic HTML.** Use `<header>`, `<section>`, `<main>`, `<footer>`, `<nav>` appropriately.
- **Accessible.** Include alt text on images, sufficient color contrast (especially on dark/gradient backgrounds), proper heading hierarchy.
- **CSS-only creativity.** Achieve all visual effects with CSS — gradients, clip-path, transforms, box-shadow, text-shadow. No images for decoration.

## Profile Photo Handling

- Check if the photo filename from `my-profile.md` exists in the `images/` folder.
- If yes: use `<img src="images/filename.jpg">` with creative CSS framing (clip-path, gradient border, artistic shadow).
- If no photo or file not found: generate an inline SVG with the person's initials (first letter of first name + first letter of last name) on a dramatic gradient background with artistic styling.
