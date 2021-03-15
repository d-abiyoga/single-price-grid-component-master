# Frontend Mentor - Single price grid component solution

This is a solution to the [Single price grid component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/single-price-grid-component-5ce41129d0ff452fec5abbbc). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

## Overview
The challenge is to build single price grid component with mobile and desktop design.
This is my first attempt to submit solution for frontend mentor challenge. I follow along a youtube video from "Coder Coder" [Building a pricing block with HTML & Pure CSS](https://youtu.be/DGYMErzcflw) with several changes.

### The challenge

Users should be able to:
- View the optimal layout for the component depending on their device's screen size
- See a hover state on desktop for the Sign Up call-to-action

### Screenshot

![Desktop design screenshot](/solution-screenshot/solution-desktop-design.png)
![Mobile design screenshot](/solution-screenshot/solution-mobile-design.png)

### Links

- Solution URL: [Solution URL](https://github.com/d-abiyoga/single-price-grid-component-master)
- Live Site URL: [Live site URL](https://d-abiyoga.github.io/single-price-grid-component-master/)

## My process
I used the youtube video mentioned in overview section as guidance to do the challenge.
First of all, I am using the  

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned

I learned the use of media query to create responsive design.
In this case I use break point of 1280px or 80rem to separate desktop design and mobile design.
```css
@media only screen and (min-width: 40rem) {
    /* Fill with code for desktop design */
    }
}
```

I learned the hover state should have vendor prefixes stated for compatibility in all supporting browsers.
The transition properties should be written in the element itself, not in the :hover state.
If the transition properties is specified in the :hover state, then transition will not work during hover-off.
```css
.subscription #sign-up{
    -webkit-transition: background-color 0.5s ease-out;
    -moz-transition: background-color 0.5s ease-out;
    -o-transition: background-color 0.5s ease-out;
    transition: background-color 0.5s ease-out;
}

.subscription #sign-up:hover{
    background-color: var(--half-transparent-yellow);
    cursor: pointer;
}
```

### Continued development

In further project / challenge, I would like to learn further the use cases for grid and flexbox layout concept.

### Useful resources

- [Building a pricing block with HTML & PuRe CSS](https://youtu.be/DGYMErzcflw) - This guide me step by step how an experienced developer do project/challenge.
- [animation](https://css-tricks.com/almanac/properties/a/animation/) - This is the article where I learn how to apply animation.

## Author

- Frontend Mentor - [@d-abiyoga](https://www.frontendmentor.io/profile/d-abiyoga)

## Acknowledgments

I would like to thank  "Coder Coder" for the youtube video [Building a pricing block with HTML & Pure CSS](https://youtu.be/DGYMErzcflw) that helps self learner like me to understand workflow of doing front end development.