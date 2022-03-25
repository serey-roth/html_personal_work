# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](/images/nft-desktop-design.png)

### Links

- Solution URL: [Solution Link](https://serey-roth.github.io/nft-preview-card-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

This is my first project working with the HTML5 markup language, CSS and Flexbox. I have gained a lot from doing this challenge, and although it's not perfect, I'm very happy with what I came up with.

Throughout this challenge, I've learned how to use CSS pseudo-classes properly to style my HTML5 elements. As one can see below, I used the before and after pseudo classes to write the hover state css code for my image. 

```css
#card-image:before {
    content:"";
    width: 302px;
    height: 302px;
    ...
    opacity: 0;
    transition: 0.35s ease-in-out; 
    z-index: 1;
}
#card-image:after {
    content: url(/images/icon-view.svg);
    width: 302px;
    height: 302px;
    ...
    display: flex;
    justify-content: center;
    align-items: center; 
    opacity: 0;
    z-index: 2;
}
#card-image:hover:before,
#card-image:hover:after {
    opacity: 0.7;
}
```

While figuring out the interactive element of the image, I became more familiar with different properties of CSS flexbox, particularly, justify-content and align-items. In this challenge, I uitilized Flexbox very heavily to align different HTML5 elements in columns and rows. I also learned about z-index and how it determines the position of the elements within a flex container. 

### Continued development

Though I'm satisfied with my work, I know the index.html looks rough so I plan on refining and making it more accessible by using the outlines of HTML5, such as section and article, where I see fit. I also want to incorporate Bootstrap into this project and make it more mobile-responsive. 

### Useful resources

- [::before / ::after](https://css-tricks.com/almanac/selectors/a/after-and-before/) - This helped me figure out how I could use before and after pseudo classes to write the hover state css code for my image.
- [A Complete Guide to Flexbox](hhttps://css-tricks.com/snippets/css/a-guide-to-flexbox/#flexbox-properties) - This is an amazing article which helped me finally understand Flexbox and its different properties. I'd recommend it to anyone still learning this concept.

### Author

Serey Ratanak Roth 
