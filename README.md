# Frontend Mentor - Meet landing page solution

This is a solution to the [Meet landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/meet-landing-page-rbTDS6OUR). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshots](#screenshot)
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

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshots

|        Mobile designed at 375px:         |        Tablet designed at 768px:         |        Desktop designed at 1440px:        |
| :--------------------------------------: | :--------------------------------------: | :---------------------------------------: |
| ![](./screenshots/screenshot-mobile.png) | ![](./screenshots/screenshot-tablet.png) | ![](./screenshots/screenshot-desktop.png) |

### Links

- Solution URL: [https://github.com/elisilk/meet-landing-page](https://github.com/elisilk/meet-landing-page)
- Live Site URL: [https://elisilk.github.io/meet-landing-page/](https://elisilk.github.io/meet-landing-page/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

- how to structure the HTML - what is the header? footer? sections?
- [Hug vs. Fill in Figma](https://bootcamp.uxdesign.cc/hug-content-or-fill-container-from-zero-to-hero-of-responsive-designs-be036e8a21ba)
- [Drawing Decorative Lines With CSS](https://pqina.nl/blog/drawing-decorative-lines-with-css/) - how to make the numbered sections with the circle and vertical line
- how to position the hero image
- [Responsive Images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)
- [Responsive images](https://web.dev/learn/design/responsive-images)
- [Responsive Images 101](https://cloudfour.com/thinks/responsive-images-101-definitions/)
- [Setting Height And Width On Images Is Important Again](https://www.smashingmagazine.com/2020/03/setting-height-width-images-important-again/)
- [Preventing a Grid Blowout](https://css-tricks.com/preventing-a-grid-blowout/)
- [CSS Image Centering – How to Center an Image in a Div](https://www.freecodecamp.org/news/how-to-center-an-image-in-a-div-css/)
- [Keep image height and hide its overflow part when it is wider than its container](https://stackoverflow.com/questions/48940673/keep-image-height-and-hide-its-overflow-part-when-it-is-wider-than-its-container)
- [Basic concepts of flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout/Basic_concepts_of_flexbox)

### Continued development

- Utilize `clamp` to implement fluid typography wherever there is a font size change across viewport sizes.
  - [https://css-tricks.com/a-complete-guide-to-calc-in-css/](https://css-tricks.com/a-complete-guide-to-calc-in-css/)
  - [min(), max(), and clamp() are CSS magic!](https://css-tricks.com/min-max-and-clamp-are-css-magic/)
- In my current implementation, the hero image is absolutely positioned, and to make that work requires knowing (or setting) the height of the container. That leads to an abrupt change from one image to the next when moving from the mobile view to the table view with the media query. But could there be a better way? I'm not sure at the moment, but want to look more into different techniques for absolute centering, and possibly combining with what I'm learning about using the `clamp` function for fluid typography, maybe. Here are some resources on absolute centering that I'd like to consider:
  - [Absolute Horizontal And Vertical Centering In CSS](https://www.smashingmagazine.com/2013/08/absolute-horizontal-vertical-centering-css/)
  - [Absolute Centering CodePen](https://codepen.io/shshaw/details/kOxGQa)
  - [Flexbox Is As Easy As Pie: Designing CSS Layouts](https://www.smashingmagazine.com/2013/05/centering-elements-with-flexbox/)

A possible better solution for dynamically sizing the hero image based on the width of the container while still allowing it to overflow the container to some extent. I recommended this kind of approach in [my comment an another person's solution](https://www.frontendmentor.io/solutions/meet-landing-page-scss-bem-grid-flexbox-zztleF0Y-Q):

```css
margin-inline-start: clamp(-2rem, calc((820px - 100vw) / -2), 0px);
```

### Useful resources

- [MDN Web Docs](https://developer.mozilla.org/en-US/) - Amazing, as always.

## Author

- Website - [Eli Silk](https://github.com/elisilk)
- Frontend Mentor - [@elisilk](https://www.frontendmentor.io/profile/elisilk)
