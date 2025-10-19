# Team Megaminds FLL Website - Copilot Instructions

## Project Overview
This is a **FIRST LEGO League (FLL) team website** for Team Megaminds' 2025 UNEARTHED season project "EARTHGUARD". The site showcases team members and their innovative coastal archaeology preservation project using LIDAR drones and carbon capture barriers.

## Architecture & Structure

### Dual Implementation Pattern
The project maintains **two parallel implementations**:
- `src/` - Main implementation with inline CSS (production-ready)
- `src/docs/` - Mirror implementation with external CSS files (for GitHub Pages)

**Key files:**
- `src/index.html` - Team member showcase (inline styles)
- `src/project.html` - Project EARTHGUARD details (inline styles) 
- `src/css/styles.css` - External CSS (simple grid-based styles)
- `src/js/main.js` - Currently empty placeholder

### LEGO-Themed Design System
The website uses a distinctive **LEGO-inspired design language**:

```css
:root {
  --lego-red: #D91E1E;
  --lego-blue: #0055BF; 
  --lego-yellow: #FFD700;
  --lego-green: #00A651;
  --lego-orange: #FF6700;
  --accent: #00f2ff; /* Neon cyan for tech elements */
}
```

**Visual patterns:**
- Cards with `--brick-shadow` (layered shadows mimicking LEGO bricks)
- LEGO brick connectors (`card::before` pseudo-elements)
- Gradient text effects for headings
- Poppins font throughout
- Dark space theme with purple gradients

### Team Structure Representation
The site reflects FLL team organization:
- **Leadership:** Coach (Nitin), Co-Coach (Phani), Team Lead (Aarav)  
- **Project Team:** Research & presentation (Lishitha, Samaira, Agrima)
- **Coding Team:** Programming & algorithms (Aarav, Sanika, Jai)
- **Building Team:** Mechanical design & assembly (Samirth, Vihaan, Aakshi)

## Development Conventions

### Navigation Pattern
Simple two-page navigation with active state styling:
```html
<nav>
  <div class="logo">TEAM MEGAMINDS</div>
  <ul>
    <li><a href="index.html" class="active">Team</a></li>
    <li><a href="project.html">Project</a></li>
  </ul>
</nav>
```

### CSS Organization
- **Inline styles** in main files for simplicity
- **CSS custom properties** for consistent theming
- **Mobile-first responsive** with `@media(max-width:900px)`
- **Animation patterns:** floating cards, glow effects, hover transforms

### Content Structure Patterns
- **Hero sections** with large gradient text
- **Card-based layouts** for team members and project sections
- **Grid systems:** `.grid.three` (3 columns), `.grid.two` (2 columns)
- **Component boxes** for technical features
- **Impact cards** with emoji icons

## FLL-Specific Context

### Project EARTHGUARD Details
When editing project content, maintain these key technical aspects:
- **Problem:** Coastal archaeological site erosion due to sea-level rise
- **Solution:** LIDAR monitoring drones + carbon capture barriers
- **Demo:** LEGO model with ultrasonic sensors and color detection
- **Impact:** UN SDG alignment (Goals 13 & 15)

### Team Workflow
- No build process required - direct HTML/CSS/JS
- Files can be opened directly in browser
- GitHub Pages deployment from `src/docs/` folder

## Editing Guidelines

1. **Preserve LEGO aesthetic** - maintain color scheme and brick-like visual elements
2. **Keep dual implementations in sync** when making major changes
3. **Use semantic HTML** with proper heading hierarchy  
4. **Maintain responsive design** - test mobile breakpoints
5. **Follow FLL values** - emphasize discovery, innovation, impact, inclusion, teamwork, fun

## Quick Reference

- **Font:** Poppins (Google Fonts)
- **Layout:** CSS Grid + Flexbox
- **Icons:** Emoji-based (🤖 🔧 ⚙️ etc.)
- **Animations:** CSS keyframes for glow, float, hover effects
- **Mobile breakpoint:** 900px
- **Max container width:** 1200px