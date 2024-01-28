# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

(./screenshots/mobile-screenshot.jpg)
(./screenshots/desktop-screenshot.jpg)

### Links

- Solution / Live Site URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

I started by laying out all the HTML first, trying to think about how to structure the containers I would be using and what the appropriate semantic choice should be for each tag. I did give many elements a class, which in retrospective was perhaps a little unnecessary given the limited scope of the project.

Coming on to CSS, I spent a while (too long) trying to figure out the best way of sizing the image relative to the container. With this eventually solved, it was then quite straightforward to go on to style the rest of the elements. I went through everything with a top-down approach, and I went back and tweaked things as the design progressed. I also added some hover states for the buttons.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

```html - making the author's profile picture and name into a single button was a last minute decision, but I feel it was a nice finishing touch:
<button class="author" onclick="authorPosts()">
  <img src="./assets/images/image-avatar.webp" alt="Greg Hooper profile picture" class="author-img">
  <h3 class="author-name">Greg Hooper</h3>
</button>
```
```css - this section of the .container style that sets it in the center of the viewport:
.container {
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
```
```css - also, this style on the image that allows for correct dynamic resizing per the design images:
.illustration {
    margin-left: auto;
    margin-right: auto;
    max-width: 100%;
    max-height: 100%;
    object-fit: cover;
    height: 220px;
    width: auto;
}
```
```js - just a really simple function as nothing really needs to happen on the page, other than open links to other pages:
function categoryFilter() {
    alert("Clicking this would open a filtered list of blog posts with this category.");
}
```

### Continued development

Some areas I would like to continue to learn more about are:
- Semantic HTML - I still don't feel fully confident with correct semantics. For example, I was very unsure what the correct tag would be for the date on the blog post, but decided to go with a <p> element - apparently a <time> tag is actually more appropriate, so I ended up changing this.
- Greater familiarity with CSS - CSS obviously has a few quirks and non-obvious ways of achieving things, so I think some more experience would really help to build confidence in knowing how to approach certain problems. Resizing the image in this project correctly was definitely a bit confusing and took a while to figure out.
- It would be great to work on some projects that need more JavaScript funcitonality to get more practice of incorporating scripted elements into a webpage.

### Useful resources

- [HTML 5 Cheat Sheet](https://html.com/blog/html-5-cheat-sheets/) - Something I will definitely be referring to going forward!
- [W3 Schools CSS object-fit Page](https://www.w3schools.com/css/css3_object-fit.asp) - This was very helpful for learning about image resizing.

## Author

- Website - [carderBee](https://carderbeebeebee.github.io/)
- Frontend Mentor - [@carderBeeBeeBee](https://www.frontendmentor.io/profile/carderBeeBeeBee)

## Acknowledgments

Chris Coyler, for his great article on how to center an element in the middle of the viewport (https://css-tricks.com/quick-css-trick-how-to-center-an-object-exactly-in-the-center/).
