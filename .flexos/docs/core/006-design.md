---
id: "006-design"
title: "Design System"
type: doc
subtype: core
status: complete
sequence: 6
tags: [ui, branding, tailwind]
---

# Design System

> Visual identity guidelines derived from the design brief to ensure authoritative and modern branding.

## Color Palette

- **Primary (Navy):** `#1B365D` - Used for headers, primary buttons, and footer.
- **Accent (Gold):** `#C5A059` - Used for primary CTAs, borders, and active states.
- **Secondary (Slate):** `#4A5568` - Used for body text, subheadings, and UI elements.
- **Background:** `#FBFBFB` - Off-white for a clean, paper-like reading experience.
- **Neutral:** `#FFFFFF` (Card backgrounds) / `#000000` (Headings).

## Typography

- **Headings:** `Playfair Display` (Serif)
    - Usage: H1, H2, H3, and Hero statements. Conveys tradition and legal authority.
- **Body:** `Inter` (Sans-serif)
    - Usage: Paragraphs, UI labels, navigation. Ensures high readability on screens.

## Component Patterns

### Buttons
- **Primary:** Background `#1B365D`, Text White, Hover darken.
- **Secondary/Accent:** Border `#C5A059`, Text `#1B365D`, Background Transparent.

### Cards (Practice Areas)
- **Style:** White background, subtle shadow (`shadow-md`), `#1B365D` top border strip.
- **Interaction:** Lift effect on hover (`transform -translate-y-1`).

### Forms
- **Input:** White background, `#4A5568` border (thin), focus ring `#C5A059`.
- **Labels:** `Inter`, font-weight medium, `#1B365D`.

## Spacing & Layout
- **Container:** Max-width `1280px` (standard desktop).
- **Section Spacing:** `py-16` or `py-24` (Tailwind scale) to allow content to breathe.
- **Grid:** 12-column grid system for desktop, collapsing to single column for mobile.