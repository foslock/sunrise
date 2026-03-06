# SUNRISE™ — The Future of Morning

A single-page satirical startup landing page for the world's most disruptive daily phenomenon: the sunrise.

## Overview

SUNRISE™ is a pure HTML/CSS/JS promotional site that parodies Silicon Valley startup culture. It features a scroll-linked animated hero that simulates a real sunrise, paired with absurdist tech-startup marketing copy.

## Features

- **Scroll-driven sunrise animation** — the sky transitions from deep night through dawn purple, crimson, orange, and golden yellow to morning blue as you scroll through the hero
- **Animated sun** — rises from the horizon with rays, parallax stars fade out as daylight arrives
- **7 content sections** — hero, intro stats, features grid, testimonials, spec table, pricing, and CTA
- **Scroll-reveal animations** — sections animate in as they enter the viewport
- **Responsive layout** — adapts to mobile at ≤900px breakpoint
- **Marquee divider** — a looping horizontal text band between sections
- No dependencies, no build step, no framework

## Usage

Just open `index.html` in a browser. No server required.

```
open index.html
```

## Structure

```
sunrise/
└── index.html   # Everything: HTML, CSS, and JS in one file
```

## Tech

- Plain HTML5, CSS3, and vanilla JavaScript
- [Inter](https://fonts.google.com/specimen/Inter) via Google Fonts
- `IntersectionObserver` for scroll-reveal
- `scroll` event listener for hero animation progress
