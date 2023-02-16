# Frontend Mentor - NFT preview card component solution

This is my a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). 

![image](https://user-images.githubusercontent.com/62683935/218565024-05b6fb72-fdfd-4edb-bc4c-864d8283e4d6.png)
 

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
- Desktop active
![image](https://user-images.githubusercontent.com/62683935/218567310-8b2e18a7-e3b5-40ad-89a2-e81a54df7c50.png)

- Mobile

<img src="https://user-images.githubusercontent.com/62683935/218565928-bf3949d1-327e-494d-b768-f3cbad8fdb98.png" width="30%"/>

- Tablet
<img src="https://user-images.githubusercontent.com/62683935/218566978-5fd35af5-b7b7-4cb8-b43b-e2336bdd6a2c.png" width="30%"/>


### Links

- Live Site URL: [GitHub Page for this project](https://benector.github.io/nft-preview-card-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow


### What I learned

The most difficult part to me was center the content on desktop view, I often lack on it in my projects because I always try first  to achieve that without using flexbox. Later I found that even mobile view was not that good because I was using margin to center the content and I wanted that to be automated. I found easier to use flexbox then, ```align-items``` solves almost all the problems and I think it worked well, but if there's a better way to do this I really wanna know and save the knowledge for life.  I have the thought that the most I can work with "pure old css" the more skilled  I am , that's why I try the hardest first, but maybe that's not the way, I searched up for many solutions to center content and I couldn't see how they were better than using flexbox.

The second dificuld part was doing overlay, I saw solutions where the ```img```  element was turned into a ```div```  with the image itself being the background, but it seemed bad for me, specially because I'm trying to use semantic html for accessibility purposes. So I found another way using img element and a ```div``` for overlay, I learned that the parent component must be positioned as ```relative``` and then the overlay ```div``` must be ```absolute``` positioned. Sometime I noticed that the overlay element was bigger in size than the ```img``` element and it wasn't good, then I found that the img element needed the ```display:block``` property.

Also I needed change opacity color of the overlay background but there's an svg icon inside this element and it was inheriting the opacity of the overlay component, then the final effect wasn't the correct. It happend because I set the background color using hsl colors, in that way I couldn't set opacity on color so I used the opacity propety on div only but that affected the whole component, so I decide to use rgb to set opacity on background and turned opacity of the overlay component to 1, so its content would show up correctly along.


### Continued development

I want to build responsive layouts more fluently and master image manipulation and position, I also want to focus on writing better semantic html and care for acessibility. Althoug it's not in this challenge, may I get some in the future, I would to like to build good animations and transitions. This is my first challenge, although I work with frontend for some years I've never wrote about the things I built so this is something new to me and I think it's good to perpetue my knowledge, I wish I can keep up that. Also english is not my first language so I'm practicing this point too. Thanks!.

### Useful resources

- [Guide to image overlays in CSS](https://blog.logrocket.com/guide-image-overlays-css/) - This helped me to understand how to use position property to do overlays.


## Author

- Linkedin - [Beatriz Benedicto](https://www.linkedin.com/in/beatrizbenedicto/)
- Frontend Mentor - [@benector](https://www.frontendmentor.io/profile/benector)


