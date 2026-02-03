# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7).  
Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the testimonials grid section depending on their device's screen size (mobile-first responsive design)
- See hover states for interactive elements if any (not present in this challenge)

### Screenshot

![Design preview for the Testimonials grid section coding challenge](./preview.jpg)

### Links

- Solution URL: [Frontend Mentor solution link](https://www.frontendmentor.io/solutions/mobile-first-workflow-google-webfonts-helper-clamp-LuvAJ9nCGx)
- Live Site URL: [https://the-ashish-gaikwad.github.io/testimonials-grid-section-challenge-fm](https://the-ashish-gaikwad.github.io/testimonials-grid-section-challenge-fm)
  
## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties (variables with HSL raw values for easy manipulation)
- Flexbox (for profile boxes and alignment utilities)
- CSS Grid (main layout with `grid-template-areas` for responsive placement)
- Mobile-first workflow
- Utility classes with data attributes (flex alignment/justify switches)
- `@font-face` + Google Webfonts Helper for Barlow Semi Condensed
- `clamp()` for fluid container padding
- `prefers-reduced-motion` media query for accessibility

### What I learned

This challenge helped me solidify several modern CSS patterns:

- **Advanced CSS Grid usage**: Using `grid-template-areas` + multiple media queries to create an asymmetric, interesting desktop layout while keeping mobile clean and stacked. Learned how to map cards properly to match the design at different breakpoints (33em → 75em+).
- **Semantic color system**: Separating raw HSL values (`--clr-purple-500-raw`) from final variables (`--color-primary`) allows easy opacity adjustments (e.g. `hsla(var(--clr-purple-500-raw), 0.1)`) and future theme changes (dark mode prep).
- **Utility-first mindset**: Created reusable `.flex` and `.stack` utilities with data attributes (`data-align`, `data-justify`) and CSS variables (`--gap`, `--gutter`). This keeps HTML declarative and reduces custom CSS.
- **Modern reset & typography**: Added `text-wrap: balance` on headings and `text-wrap: pretty` on paragraphs. Used font shorthand + rem units consistently. Switched author name to rem instead of px.
- **Quotation SVG positioning**: Used `position: absolute` + `z-index: -1` on the decorative quote SVG (only visible on larger screens for the first card).
- **Accessibility basics**: Respected `prefers-reduced-motion`, good alt text, semantic `<main>`, focus-within + smooth scroll (with override).
- **Line endings awareness**: Encountered Git LF/CRLF warning on Windows → learned about `core.autocrlf` and `.gitattributes` for cross-platform consistency.

### Continued development

In future projects I want to focus on:

- Mastering more complex grid patterns (auto-fit, minmax, subgrid)
- Building a full design system with even more semantic tokens (spacing scale, shadow scale)
- Adding dark mode toggle using the HSL raw values
- Improving performance audits (font loading, image optimization)
- Writing more robust media query strategies (fewer breakpoints, container queries if applicable)
- Exploring logical properties (`padding-inline`, `margin-block`) for better RTL support

### Useful resources

- [CSS Grid - grid-template-areas explained (MDN)](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-template-areas) — Great reference for named areas
- [Modern CSS Reset by Andy Bell](https://piccalil.li/blog/a-modern-css-reset/) — Inspired parts of my reset
- [Google Webfonts Helper](https://gwfh.mranftl.com/fonts) — Easy self-hosted @font-face generation
- [clamp() Generator](https://fluidtypography.com/) — Helped tune container padding
- [Kevin Powell YouTube - CSS Grid mastery](https://www.youtube.com/c/KevinPowell) — Excellent Grid tutorials

## Author

- Frontend Mentor - [@the-ashish-gaikwad](https://www.frontendmentor.io/profile/the-ashish-gaikwad)
- GitHub - [https://github.com/the-ashish-gaikwad](https://github.com/the-ashish-gaikwad)

---

Thanks for checking out my solution! Feedback is always welcome.
