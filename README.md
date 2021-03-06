# Frontend Mentor - Advice generator app solution

This is a solution to the [Advice generator app challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/advice-generator-app-QdUG-13db). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)


## Overview

### The challenge

Users should be able to:
  - Use from any device.
  - Get API advice by clicking the button 

### Screenshot

![](screenshot.PNG)


### Links

- Live Site URL: [Add live site URL here]( https://vittor-emanoel.github.io/Advice-generator-app-main/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Use API



### What I learned


```js
 fetch('https://api.adviceslip.com/advice')
    .then((response) => {
      return response.json();
    })
    .then((adviceData) => {
      const adviceNum = adviceData.slip.id;
      const adviceText = adviceData.slip.advice;

      adviceNumber.textContent = adviceNum;
      adviceContent.textContent = adviceText;
    })
    .catch((error) => {
      console.log(error);
    });
```


## Author

- Frontend Mentor - [@Vittor](https://github.com/Vittor-Emanoel)


