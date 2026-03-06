# CLAUDE.md

## Project overview

Single-file satirical startup landing page (`index.html`). All HTML, CSS, and JavaScript live in one file — no build tools, no dependencies, no framework.

## Key architecture

- **Hero animation** — driven by a `scroll` event listener that maps scroll progress (0–1) to sky gradient stops, sun position, and star opacity. See `#skyBg`, `#sunWrap`, `#starsLayer` elements and the `onScroll()` function.
- **Scroll-reveal** — `IntersectionObserver` toggles the `.visible` class on `.reveal` elements as they enter the viewport.
- **Marquee divider** — CSS `animation: marquee` on `.marquee-track` (duplicated content for seamless loop).
- **Responsive breakpoint** — `@media (max-width: 900px)` at the bottom of the `<style>` block.

## Editing guidelines

- All styles are in the `<style>` block in `<head>`. CSS is organized with section comments like `/* ── HERO ── */`.
- All JavaScript is in a single `<script>` block at the end of `<body>`.
- The sunrise color sequence (used in `onScroll()`) goes: deep night → dawn purple → crimson → orange → golden yellow → morning blue. Preserve this order when adjusting colors.
- The marquee section (`.marquee-section`) is a mid-page divider, separate from the removed bottom ticker.

## No build step

Open `index.html` directly in a browser to preview changes.
