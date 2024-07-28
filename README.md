# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents


  - [Screenshot](#screenshot)
  - [Links](#links)
  - [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
 


### Screenshot


![Desktop](/nft-preview-card-component-main/desktop-screenshot.png?raw=true)
![Desktop active](/nft-preview-card-component-main/desktop-active.png?raw=true)

![Mobile](/nft-preview-card-component-main/mobile-screenshot.png?raw=true)
![Mobile active](/nft-preview-card-component-main/mobile-active.png?raw=true)


### Links

- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

This is my first time using svg images and practicing building a site from a design using only HTML and CSS. I've had a struggle with the active stats of the main image, but I found a solution in the internet that worked very well, at least at these specified layout sizes: 

mobile: (Iphone SE: 375x667)
desktop: (Notebook Ideapad Lenovo: 1920x1080)

Please use these specified layouts to see the results.

It was nice to use flexbox, margins and paddings to position the content. I still looking for another solutions for the overlay image when clicked, mainly because my solution work only in two specific layouts. Here's the code for the active part of the project:

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

```html
<div class="overlay">
  <img class="hoverImg" src="/nft-preview-card-component-main/images/icon-view.svg" alt="view">
</div>
```

```css
.overlay {
    position: absolute;
    top: 65px;
    bottom: 0;
    left: 48px;
    right: 0px;
    height: 42%;
    width: 74.5%;
    opacity: 0;
    transition: .5s ease;
    background-color: var(--cor-texto2);
    border-radius: 0.5rem;
}
.container:hover .overlay {
    opacity: 1;
    cursor: pointer;
}
.hoverImg {
    width:15%;
    position: absolute;
    left: 120px;
    top: 120px;
}
```

