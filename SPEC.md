# Earth Love United (ELU) Website Specification

## Concept & Vision

A commanding, authoritative digital presence for a global regenerative sustainability foundation. The site conveys credibility, scale, and impact through restrained elegance—letting the mission speak while the design communicates professionalism and forward-thinking innovation. Dark, immersive, with strategic pops of mint and cyan that suggest environmental renewal and technological progress.

## Design Language

### Aesthetic Direction
Minimal dark luxury meets environmental tech. Think Bloomberg Terminal meets Patagonia—data-driven credibility with planetary purpose. No decorative clutter; every element earns its place.

### Color Palette
- **Background Dark**: `#0A0E0C`
- **Mint Accent**: `#7DF9C8`
- **Cyan Accent**: `#00CED1`
- **Gradient**: `linear-gradient(135deg, #7DF9C8 → #00CED1)`
- **Text Primary**: `#F8FBFA`
- **Text Muted**: `rgba(248,251,250,0.6)`
- **Card Background**: `rgba(255,255,255,0.03)`
- **Border Subtle**: `rgba(255,255,255,0.08)`

### Typography
- **Display**: Playfair Display (serif) — headlines, hero text
- **Body**: Inter (sans-serif) — all body copy, UI elements
- **Scale**: 4rem hero, 2.5rem section titles, 1.125rem body, 0.875rem muted

### Spatial System
- Section padding: 6rem vertical
- Container max-width: 1200px
- Card padding: 2rem
- Grid gap: 2rem
- Border radius: 12px (cards), 8px (buttons), 4px (inputs)

### Motion Philosophy
- All transitions: 0.25s ease (buttons, cards), 0.3s ease (nav underline)
- Hover states: subtle lift (translateY -4px), glow effects on accents
- Scroll-triggered fade-in for sections (optional enhancement)
- No gratuitous animation—motion serves feedback

### Visual Assets
- Icons: Lucide icons via CDN (line style, 1.5px stroke)
- Team avatars: Initials in gradient-bordered circles
- No decorative images or orbs
- Strategic use of gradient text for emphasis

## Layout & Structure

### Page Flow
1. **Navigation** — Fixed top, transparent → solid on scroll
2. **Hero** — Full viewport impact, centered content, gradient accents
3. **About** — Mission statement, 3-column value points
4. **Mission & Vision** — Centered text block with vision card
5. **Research** — 3×2 card grid showcasing projects
6. **ELU Token** — Split layout: features list + stats card
7. **Carbon Portfolio** — Bold stat hero + info cards
8. **Team** — 3-column member cards
9. **Contact** — Form + details side by side
10. **Footer** — Links, copyright, minimal

### Responsive Strategy
- Desktop: Full layouts, 3-column grids
- Tablet (≤1024px): 2-column grids, adjusted spacing
- Mobile (≤768px): Single column, stacked layouts
- Small mobile (≤480px): Compact spacing, full-width cards

## Features & Interactions

### Navigation
- Fixed position, blur backdrop
- Logo left, nav links right
- Hover: underline slides in from left (gradient)
- Mobile: hamburger menu with slide-down panel

### Hero Section
- Eyebrow text with gradient
- Large serif headline
- Subtext paragraph
- Two CTAs: primary (gradient) + secondary (outline)
- Stats row: 3 metrics with icons

### Cards (Research, Team, Info)
- Subtle border, transparent background
- Hover: border brightens, slight lift, accent glow
- Icon or avatar at top
- Title + description

### Form Inputs
- Dark background with subtle border
- Focus: border becomes gradient, subtle glow
- Labels above inputs
- Submit button: gradient background, hover brighten

### Buttons
- Primary: gradient background, white text
- Secondary: transparent, gradient border
- Hover: brightness increase, slight scale

## Component Inventory

### Nav Link
- Default: muted text color
- Hover: white text, underline animates in
- Active: white text, underline visible

### Primary Button
- Default: gradient bg, white text, rounded
- Hover: brightness 110%, translateY -2px
- Active: brightness 90%

### Secondary Button
- Default: transparent, gradient border, gradient text
- Hover: bg fills with gradient at 10% opacity
- Active: border brightens

### Card
- Default: rgba bg, subtle border, rounded
- Hover: border brightens to mint, translateY -4px, shadow glow
- Contains: icon/avatar, title, description

### Input Field
- Default: dark bg, subtle border, muted placeholder
- Focus: gradient border, white text, subtle glow
- Error: red border (if validation needed)

### Team Avatar
- Circle with gradient border
- Initials centered in white
- Size: 80px diameter

## Technical Approach

- **Stack**: Single HTML file with embedded CSS and vanilla JavaScript
- **Fonts**: Google Fonts (Playfair Display 400/600, Inter 400/500/600)
- **Icons**: Lucide icons via CDN
- **No frameworks** — pure HTML/CSS/JS for maximum performance
- **CSS**: Custom properties for theming, flexbox/grid for layout
- **JS**: Minimal — mobile nav toggle, smooth scroll, form handling