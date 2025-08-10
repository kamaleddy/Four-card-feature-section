# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](./screenshot/Desktop%20View.png)
![](./screenshot/Mobile%20View.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [live site URL here](https://kamaleddy.github.io/Four-card-feature-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

In this project I learned how to use responsive grid that adapts with `auto-fit` and uses `minmax()` for flexibility sizing. In media queries, it becomes a 6-column custom layout.

This is how I do it, see below:

```css
.features {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(auto, 1fr));
  gap: 2rem;
}

@media (min-width: 52em) {
  .features {
    grid-template-columns: repeat(6, 1fr);
  }

  .one {
    grid-column: 1 / span 2;
    grid-row: 2 / span 2;
  }

  .two {
    grid-column: 3 / span 2;
    grid-row: 1 / span 2;
  }

  .three {
    grid-column: 3 / span 2;
    grid-row: 3 / span 2;
  }

  .four {
    grid-column: 5 / span 2;
    grid-row: 2 / span 2;
  }
}
```

### Continued development

In this project right now I`m using grid column and row numbers, in the next project i want to start using named grid areas instead of numeric positioning, which makes the grid’s structure easier to read and adjust.

### Useful resources

- [Guide to CSS Grid](https://www.joshwcomeau.com/css/interactive-guide-to-grid/) - This helped me understand about grid and and how used it and apply on this project. Its give clearer explanation with example by adding a small code snippet and a visual analogy.

## Author

- Github - [@kamaleddy](https://github.com/kamaleddy)
- Frontend Mentor - [@kamaleddy](https://www.frontendmentor.io/profile/kamaleddy)
