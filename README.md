# Liquid Lounge 🍸

A modern, animated cocktail landing page built with React and GSAP. Liquid Lounge focuses on an immersive, responsive UI with smooth animations and micro-interactions to create a memorable product landing experience.

---

## Demo

- Live demo: https://liquid-lounge.vercel.app

---

## Features

- Smooth, performant animations powered by GSAP (GreenSock Animation Platform)
- Built with React for component-driven structure
- Fully responsive layout for mobile, tablet, and desktop
- Immersive hero and section transitions with scroll-triggered animations
- Accessible markup and keyboard-friendly interactions where applicable
- Easy-to-customize theme and content (colors, typography, copy)

---

## Tech Stack

- React
- GSAP (GreenSock) — animation engine
- CSS (flexbox/grid + responsive utilities)
- HTML5

(Adjust this list if you use Vite, Create React App, Tailwind, or other tooling.)

---

## Getting Started

These instructions assume a standard Node.js + npm workflow. If your project uses yarn or pnpm, swap the commands accordingly.

1. Clone the repo
   git clone https://github.com/habib-design/liquid_lounge.git
2. Install dependencies
   npm install
3. Run the dev server
   npm run dev
4. Open http://localhost:3000 (or the port your setup uses)


---

## Development Notes

- Animation structure: GSAP timelines are used to sequence hero, section, and micro-interaction animations. Look for timeline setup in components like `Hero.jsx`, `Animations/*`, or `useAnimations.js`.
- Scroll triggers: If using GSAP ScrollTrigger, ensure it is properly registered and scoped to component mount/unmount to avoid memory leaks in React.
- Refs: Many animated elements use React refs. Keep DOM queries minimal and prefer refs for stable performance.

Tips:
- When adding new animations, wrap them in short timelines and kill them on unmount.
- Use `gsap.context()` (GSAP 3.11+) inside React components to scope selectors and cleanup automatically.

---

## Customization

- Theme colors and fonts live in  `src/index.css`. Update variables to quickly re-theme the site.
- Replace copy, images, and icons in `public/` and component props to match your brand.
- For additional pages, add routes and reuse animation components where appropriate.

---

## Accessibility & Performance

- Ensure animated content remains readable and navigable by keyboard users.
- Provide reduced-motion preferences: check `prefers-reduced-motion` and disable/soften non-essential animations accordingly.
- Optimize images (use modern formats, lazy loading) and avoid animating large layout properties—prefer transforms and opacity for better performance.

---

Common steps:
1. Build: npm run build
2. Deploy build directory to chosen host
3. Configure redirects or single-page fallback if using client-side routing

---


## Acknowledgements

- GSAP (GreenSock) for the animation library
- Design inspiration and any asset attributions

---

## Contact

Project maintained by habib-design (GitHub).
