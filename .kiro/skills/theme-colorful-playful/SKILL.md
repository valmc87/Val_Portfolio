---
name: theme-colorful-playful
description: Generate a colorful and playful personal branding website. Use when the attendee wants bold colors, rounded shapes, and fun fonts. Reads my-profile.md for content.
---

# Theme: Colorful & Playful 🎨

Generate a single-page personal branding website with a **colorful, playful, and energetic** visual style.

## Content Source

Read `my-profile.md` in the project root for all personal content (name, tagline, bio, skills, experience, achievements, fun facts, social links, and profile photo filename).

## Files to Generate

1. `index.html` — the complete single-page website
2. `style.css` — all styles in a separate stylesheet

## Visual Style Requirements

- **Color palette:** Use vibrant, bold colors — think coral, teal, sunny yellow, electric purple. Use at least 3–4 accent colors.
- **Shapes:** Rounded corners everywhere (border-radius: 15px+). Use pill-shaped buttons and tags.
- **Fonts:** Use Google Fonts — pick a fun heading font (e.g., Poppins, Fredoka One, Baloo 2) and a clean body font (e.g., Nunito, Quicksand).
- **Layout:** Use a card-based layout. Each section is a colorful card with subtle shadows.
- **Emojis:** Sprinkle relevant emojis in section headings (e.g., "✨ About Me", "🚀 Skills", "🎯 Achievements").
- **Background:** Light background with colorful accents or subtle patterns.
- **Hover effects:** Cards should have a gentle lift/scale on hover.

## Section Structure

Build these sections in order, using content from `my-profile.md`:

### 1. Hero / Header
- Large, bold name
- Tagline underneath
- Profile photo in a circle with a colorful border (if photo exists in `images/` folder, use it; otherwise generate an SVG placeholder with the person's initials and a bright gradient background)
- Fun background — gradient or colorful shapes

### 2. About Me
- The bio text from my-profile.md
- Styled as a highlighted card

### 3. Skills & Passions
- Display as colorful pill-shaped tags/badges
- Each skill gets a different accent color

### 4. Experience / Education
- Timeline or stacked card layout
- Each entry is a mini card with role, company/school, and dates

### 5. Achievements
- Icon or emoji + achievement text
- Could be a grid of small cards or a list with visual flair

### 6. Fun Facts
- Playful layout — could be speech bubbles, sticky notes, or a fun grid
- Each fact gets its own colorful container

### 7. Social Links
- Large, colorful icon buttons for each platform
- Use inline SVG icons or Unicode symbols (no external icon libraries to keep it simple)
- Hover effect: scale up or color shift

### 8. Footer
- Simple footer with "Built with 💜 and AI at Women In Tech Workshop"
- Include #GivetoGain

## Technical Requirements

- **Pure HTML + CSS only.** No JavaScript. No frameworks. No build tools.
- **Mobile responsive.** Must look good on phones (use CSS flexbox/grid, media queries).
- **Single page.** Everything in one `index.html`.
- **External stylesheet.** All CSS in `style.css`, linked from `index.html`.
- **Google Fonts.** Import via `<link>` tag in HTML head.
- **No external dependencies** other than Google Fonts.
- **Semantic HTML.** Use `<header>`, `<section>`, `<main>`, `<footer>`, `<nav>` appropriately.
- **Accessible.** Include alt text on images, sufficient color contrast, proper heading hierarchy.

## Profile Photo Handling

- Check if the photo filename from `my-profile.md` exists in the `images/` folder.
- If yes: use `<img src="images/filename.jpg">` with a circular clip and colorful border.
- If no photo or file not found: generate an inline SVG circle with the person's initials (first letter of first name + first letter of last name) on a bright gradient background. Use a large, bold, white font for the initials.
