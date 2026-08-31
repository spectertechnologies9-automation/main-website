# Specter Automations

A premium, dark, editorial one-page site for **Specter Automations** — an AI
automation and technology studio. Built with React + Vite, Framer Motion, and
Lenis for smooth scrolling.

This project was rebuilt as a learning/reference exercise: the overall layout,
typographic hierarchy, spacing rhythm, navigation behavior, and interaction
language (hover states, scroll reveals, cursor behavior, editorial project
rows) follow the visual language of a reference portfolio site, reimplemented
from scratch with original code, copy, and a new brand identity/color system.

## Stack

- React 19 + Vite
- Framer Motion (page-load choreography, scroll reveals, hover states)
- Lenis (smooth scrolling)
- Plain CSS with a small design-token system (`src/index.css`)

## Structure

```
src/
  components/
    Navbar.jsx / Navbar.css        top navigation + mobile menu
    Hero.jsx / Hero.css            hero statement + intro copy
    Projects.jsx / ProjectItem.jsx editorial "selected work" list
    Services.jsx                   typography-driven services list
    About.jsx                      editorial about statement
    Contact.jsx                    closing CTA + links
    Footer.jsx                     copyright + back-to-top
    Cursor.jsx                     custom cursor (desktop only)
    Preloader.jsx                  load-in sequence
    SideBadge.jsx                  fixed availability badge
    Ambient.jsx                    background grain/glow layer
    Reveal.jsx                     shared scroll-reveal primitives
  hooks/
    useLenis.js                    smooth-scroll setup + scrollToTarget helper
```

## Running locally

```bash
npm install
npm run dev       # start dev server
npm run build     # production build to dist/
npm run preview   # preview the production build
```

## Notes

- The custom cursor and Lenis smooth scrolling are disabled automatically on
  touch devices.
- All project imagery is CSS-generated placeholder artwork — swap the
  `.swatch-*` backgrounds in `Projects.css` for real project imagery when
  available.
- Copy, branding, palette, and all "projects" are fictional content created
  for Specter Automations and do not reference the original reference site's
  content, images, or code.
