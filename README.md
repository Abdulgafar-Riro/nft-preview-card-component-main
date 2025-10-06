# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U).  
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
- [Acknowledgments](#acknowledgments)

---

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements (image overlay, title, and author name)

### Screenshot

![](./images/screenshot.jpg)

_(Add your final design screenshot here — ideally cropped around the card component.)_

### Links

- **Solution URL:** [Add your solution URL here](https://your-solution-url.com)
- **Live Site URL:** [Add your live demo here](https://your-live-site-url.com)

---

## My process

### Built with

- **Semantic HTML5 markup**
- **SASS (SCSS) preprocessor**
- **BEM (Block Element Modifier)** naming convention
- **Modular architecture** (Base, Layout, Components)
- **CSS Design Tokens** (colors, spacing, typography)
- **Flexbox** for alignment and layout
- **Hover transitions and image overlay effect**
- **Responsive design** (mobile-first approach)

### What I learned

This project helped me practice **SASS architecture and modular thinking**.  
I learned how to organize a scalable SCSS structure using partials and `@use`,  
and how to apply the **BEM methodology** for clear, reusable class naming.

```scss
.card {
  &__image {
    position: relative;
    overflow: hidden;

    &-overlay {
      position: absolute;
      inset: 0;
      background-color: $color-primary;
      opacity: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      transition: opacity 0.3s ease;
    }

    &:hover {
      .card__image-overlay {
        opacity: 0.5;
      }
    }
  }
}

I also gained more confidence in using SASS nesting, variables, and mixins to simplify my code.

Continued development

In future projects, I want to:

Incorporate SASS mixins and functions for responsive breakpoints and animations.

Experiment with CSS Grid for more complex layouts.

Automate my SASS workflow using Vite or Gulp for faster builds.

Useful resources

SASS Documentation
 – Great reference for @use, nesting, and variables.

BEM Methodology Guide
 – Helped me refine naming structure.

Frontend Mentor Community
 – For seeing others’ approaches to the same challenge.

Author

Name: Abdulgafar (WebMujahid)

Website: https://github.com/abdulgafar-riro

Frontend Mentor: @Abdulgafar-riro

Acknowledgments

Special thanks to the Frontend Mentor team for designing realistic and well-structured challenges.
I also appreciate the open-source community for resources that inspired my code organization.
```
