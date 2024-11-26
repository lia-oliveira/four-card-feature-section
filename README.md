# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Frontend Mentor - Four card feature section solution](#frontend-mentor---four-card-feature-section-solution)
  - [Table of contents](#table-of-contents)
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
Preview:

![](./design/desktop-preview.jpg)

My solution:

![](./design/solution-by-gillian.png)

### Links

- Solution URL: [Four Card Feature Section Repo](https://github.com/lia-oliveira/four-card-feature-section)
- Live Site URL: [Four Card Feature Section Live](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- CSS Variables


### What I learned
There were many lessons learned. Positioning elements was certainly the most significant, but the ones listed below were also important:

1 - Merging rows in a CSS grid using span.
```css
.card--1 {
    grid-column: 1;
    grid-row: 1 / span 2;
    align-self: center;
}
```

2 - Using the data-icon attribute in HTML5 to reference an icon added to the layout via CSS.

```html
<article class="card card--cyan card--1">
   ...
   <p class="card__description" data-icon="supervisor">Monitors activity to identify project roadblocks</p>
      </article>
```

```css
.card__description[data-icon="supervisor"]::after {
    content: "";
    background-image: url('./../images/icon-supervisor.svg');
    display: inline-block;
    background-size: contain;
    background-repeat: no-repeat;
    width: 64px;
    height: 64px;
    position: absolute;
    right: 3rem;
    top: calc(55% + 0.5rem);
}
```

3 - Applying BEM modifiers to change the card's header colors.
```css
.card--cyan {
    border-top: 3px solid var(--co-Primary-cyan);
}
```

### Continued development
I definitely need more practice with positioning elements using CSS Grid.


### Useful resources
The main resources I used were:

[Complete Guide Grid - CSS Tricks](https://css-tricks.com/snippets/css/complete-guide-grid/)

[CSS Grid Layout Guia Completo - Origamid](https://www.origamid.com/projetos/css-grid-layout-guia-completo/)

[CSS Grid Layout](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout)

[CSS Grid](https://www.alura.com.br/artigos/css-grid-guia-propriedades-grid-container-grid-item?srsltid=AfmBOopuPEd-vj69wAlyypzRAjRUgEEHBBGvFuyrHe4NejKAlBwhHFCX)

[CSS Flexbox Guia Completo](https://origamid.com/projetos/flexbox-guia-completo/)

## Author

- Website - [Github](https://github.com/lia-oliveira)
- Frontend Mentor - [@lia-oliveira](https://www.frontendmentor.io/profile/lia-oliveira)
- Twitter - [@byliaoliveira](https://x.com/byliaoliveira)



