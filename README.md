# AMEEN PASHA — Cinematic Portfolio

Static site (HTML / CSS / JS, GSAP + ScrollTrigger + Lenis from CDN, canvas particles). No build step.

## Deploy on GitHub Pages
1. Copy the contents of this folder into your existing portfolio repo (keep your current `CNAME` / repo settings).
2. Commit and push. Pages serves `index.html` from the repo root.
3. To preview locally, use a server (the sand effect reads the photo's pixels, which browsers block on `file://`):
   `python3 -m http.server` then open http://localhost:8000

## Add your verified details — `js/config.js`
- `contact` : email, WhatsApp number, Instagram URL and any other profiles. Empty fields are never shown.
- `SITE_WORKS` : one entry per real project (image in `assets/work/`). Categories: Graphic Design, VFX Work, Video Projects, Camera Work, Motion Graphics, Creative Projects.

## Images
- `assets/images/ameen-hero.JPG` is your untouched original (exact case preserved).
- The page uses optimized copies: `ameen-hero-web.jpg/.webp` (hero) and `ameen-hero-900.jpg` (filmmaking section).

## Structure
- `js/main.js` — scroll timeline (zoom → sand dissolve → memory world), reveals, gallery, nav
- `js/sand.js` — particle engine built from the portrait's own pixels
- `js/ambient.js` — floating dust / atmospheric light
- Reduced-motion users get a static, fully readable version.
