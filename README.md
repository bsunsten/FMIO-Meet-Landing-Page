# Frontend Mentor - Meet landing page solution

This is a solution to the [Meet landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/meet-landing-page-rbTDS6OUR). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [AI Collaboration](#ai-collaboration)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./screenshot.jpeg)



### Links

- Live Site URL: [https://bsunsten.github.io/FMIO-Meet-Landing-Page/](https://bsunsten.github.io/FMIO-Meet-Landing-Page/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- Dart Sass

### What I learned

This was honestly a pretty difficult challenge, when it came to setting the desktop styles! The biggest thing I learned about this challenge was that CSS grid actually has a minimum width to fit the content of a column. As the images were larger than the div, the computed width of the hero was ending up larger than the viewport and messing up alignment. The fix for this was to add the following line:

```
 .hero {
    grid-template-columns: minmax(0, 1fr) minmax(0, 1fr);
  }
```

The minmax is what I was missing and this was a huge revelation for me! 


### Continued development

This project took me a few days of tinkering to get to the current state. I'm not terribly happy with how close it is to the design still, but I'm excited to take on Javascript challenges. I'm not planning to refactor this, but if I were, I would want to clean up my "base" styles, as they're rather verbose and probably should be split into other files. 


### AI Collaboration

Because this desktop styling challenge was so tricky, I used Claude heavily to try and work through some issues. This was honestly a bit of a hinderance, as it kept repeating the same suggestion to me. It wasn't until I added some specific context that I figured out the CSS grid issue I mentioned above. 


