# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-N2T2BASub). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

---

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size (`Desktop` & `Mobile`).
- Experience a clean, accessible, and structured grid layout.

### Screenshot

![Testimonials Grid Section Preview](./design/desktop-preview.jpg)

### Links

- **Solution URL:** [GitHub Repository](https://github.com/kirujaxx/QR_FLEX) *(بدل هاد الرابط بالرابط ديال الـ Repo ديالك)*
- **Live Site URL:** [GitHub Pages Live Demo](https://kirujaxx.github.io/QR_FLEX/) *(بدل هاد الرابط بالـ Live Demo ديالك)*

---

## My process

### Built with

- Semantic **HTML5** markup
- **CSS3** custom properties (Variables)
- **CSS Grid** (for layout structure and area positioning)
- **Flexbox** (for alignment within components)
- **BEM Methodology** (for clean class naming)
- **CSS Pseudo-elements** (`::before` for background quotation pattern)
- Mobile-first / Desktop-responsive workflow

### What I learned

During this challenge, I sharpened my skills in using **CSS Grid** to create complex asymmetric card layouts. 

Here are some technical highlights:

1. **CSS Grid Area Mapping:** 
   Configuring explicit grid lines for desktop while cleanly resetting them for mobile screen sizes using `grid-area: auto`.

```css
.purple {
  grid-area: 1 / 1 / 2 / 3;
  background-color: var(--purple);
}

@media (max-width: 950px) {
  .purple, .grey, .white, .light-grey, .dark-blue {
    grid-area: auto;
  }
}