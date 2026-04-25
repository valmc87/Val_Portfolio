---
name: theme-clean-minimal
description: Generate a clean and minimal personal branding website. Use when the attendee wants white space, elegant typography, and a muted palette. Reads my-profile.md for content.
---

# Theme: Clean & Minimal ✨

Generate a single-page personal branding website with a **clean, minimal, and elegant** visual style.

## Content Source

Read `my-profile.md` in the project root for all personal content (name, tagline, bio, skills, experience, achievements, fun facts, social links, and profile photo filename).

## Files to Generate

1. `index.html` — the complete single-page website
2. `style.css` — all styles in a separate stylesheet

## Visual Style Requirements

- **Color palette:** Muted and restrained — off-white (#fafafa), charcoal (#333), one subtle accent color (e.g., soft blue #6C8EBF, sage green #7D9B76, or dusty rose #C4A4A4). Maximum 2 accent colors.
- **Shapes:** Clean lines, minimal border-radius (4–8px max). Thin borders or dividers between sections.
- **Fonts:** Use Google Fonts — a refined serif or sans-serif heading font (e.g., Inter, DM Sans, Playfair Display, Lora) and a clean body font (e.g., Inter, Source Sans Pro).
- **Layout:** Generous white space. Content centered with a max-width of ~700px. Breathing room between sections.
- **Background:** Pure white or very light gray. No patterns, no gradients.
- **Hover effects:** Subtle — slight color change or underline on links. Nothing flashy.
- **Overall feel:** Like a beautifully typeset document. Think Apple.com meets a designer's portfolio.

## Section Structure

Build these sections in order, using content from `my-profile.md`:

### 1. Hero / Header
- Name in large, elegant typography
- Tagline in lighter weight or smaller size underneath
- Profile photo in a clean circle or soft rounded square (if photo exists in `images/` folder, use it; otherwise generate an SVG placeholder with the person's initials on a muted background)
- Minimal layout — centered, lots of breathing room

### 2. About Me
- Clean paragraph text
- Maybe a thin top border or subtle section divider

### 3. Skills & Passions
- Simple inline list or minimal tags with thin borders
- No heavy colors — use the accent color sparingly

### 4. Experience / Education
- Clean list with clear hierarchy: role in bold, company/school in regular weight, dates in light gray
- Thin dividers between entries

### 5. Achievements
- Simple bulleted or icon-prefixed list
- Clean and scannable

### 6. Fun Facts
- Light, airy layout — could be a simple list or small cards with very subtle backgrounds
- Keep it playful but within the minimal aesthetic

### 7. Social Links
- Text links or minimal icon links in a horizontal row
- Use inline SVG icons or Unicode symbols — keep them small and elegant
- Hover: subtle underline or color shift

### 8. Footer
- Minimal footer: "Built with ✨ and AI at Women In Tech Workshop"
- Include #GivetoGain
- Small, light text

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
- If yes: use `<img src="images/filename.jpg">` with a clean circular or soft-rounded clip.
- If no photo or file not found: generate an inline SVG circle with the person's initials (first letter of first name + first letter of last name) on a muted, elegant background. Use a clean, light font for the initials.
