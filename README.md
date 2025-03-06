# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

### Screenshot

![](/assets/images/frontendmentor-RecipePage-challengeSH.PNG)


### Links

- Solution URL: [GitHub](https://github.com/Joz312v/Recipe-Page-Fend-Mentr)
- Live Site URL: [Live Preview](https://joz312v.github.io/Recipe-Page-Fend-Mentr/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [Prismic](https://prismic.io/blog/css-text-animations) - CSS Text animations Library

### What I learned

(Has nothing to do with the overall challenge, but I was just thinking of how to improvised the attribution section )

```html
<div class="attribution">
```
![](/assets/images/Frontend-Mentor-BreakText.gif)

This text hover effect by parkHJ11 gives off a sort of hamburger vibe with the “in yourself” text placed between two “believe” texts. It relies on:

clip-path: To clip the top and bottom halves of the “believe” texts on hover
CSS transforms (translateY and scaleY): To make the different text slide into view on hover
```css
h2 {
  margin: 0; padding: 0;
  position:absolute;
  top: 50%; left: 50%;
  transform:translate(-50%,-50%);
  font-size: 6em; color:transparent;
  text-transform:uppercase;
}
h2 span:nth-child(1){
  position:absolute;
  top:0; left:0; color: #000;
  transition:0.5s;
  clip-path: polygon(0 0, 100% 0, 100% 50%, 0 50%);
  overflow:hidden;
}
h2:hover span:nth-child(1){
  transform:translateY(-18px); 
}
h2 span:nth-child(2){
  position:absolute;
  top:0; left:0; color: #000;
  transition:0.5s;
  clip-path: polygon(0 50%, 100% 50%, 100% 100%, 0 100%);
  overflow:hidden;
}
h2:hover span:nth-child(2){
  transform:translateY(18px); 
}
h2 span:nth-child(3){
  position:absolute;
  top:50%; left: 0;
  transform:translateY(-50%) scaleY(0);
  width: 91%; color: #000;
  background:#ff0;
  font-size: 0.25em; font-weight: 500;
  letter-spacing:0.7em;
  text-align:center;
  padding-left: 20px; margin-left: 5px;
  transition:0.5s;
}
h2:hover span:nth-child(3){
  transform:translateY(-50%) scaleY(1);
}
```

### Continued development

You can't memorize every syntax there is, you have to have your own notes. Build something and make notes as you go.

### Useful resources

- [Prismic.io](https://prismic.io/blog/css-text-animations) - They have plenty cool collections of CSS animations


## Author

- Frontend Mentor - [@Joz312v](https://www.frontendmentor.io/profile/Joz312v)
- GitHub - [@Joz312v](https://github.com/Joz312v)


## Acknowledgments
- parkhj11 - [@codepen.io](https://codepen.io/parkhj11)
- prismic.io - [CSS Blog](https://prismic.io/blog/css-text-animations)
