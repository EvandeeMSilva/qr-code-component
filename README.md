# Frontend Mentor - QR code component

PT-BR README: [:brazil:](README-pt-br.md)

Hi there! This is my solution to: [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). 

Frontend Mentor is a platform with a lot of challenges to help you improve your coding skills by building realistic projects. 

## Table of contents

- [Frontend Mentor - QR code component](#frontend-mentor---qr-code-component)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [Screenshots](#screenshots)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [Decisions](#decisions)
    - [Updates After Challenge](#updates-after-challenge)
  - [Author](#author)
  - [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

It's a simple page of a card with a QR code in it, similar pages are used for an infinity of things; from redirecting people to other pages to making payments by reading the QR code.

### Screenshots

<details open>
  <summary>desktop view</summary>
  <img src="./screenshots/desktop-view-screenshot.png">
</details>

<details>
  <summary>Mobile view</summary>
  <img src="./screenshots/mobile-view-screenshot.png">
</details>

### Links

- Solution URL: https://github.com/EvandeeMoS/qr-code-component
- Live Site URL: https://evandeemos.github.io/qr-code-component/

## My process

### Built with

- Semantic HTML5 markup
- CSS grid layout
- Mobile-first workflow

### Decisions


I decided to use Mobile-first workflow, it was because I think this type of page applies better to mobile than desktop, I think it looks a little empty in the desktop version.

I made some plans about how I would apply things and then I just needed to implement them, it made the code flow a lot faster than I thought.

<details>
<summary>old versions</summary>
I made this page using just what I already knew about CSS and HTML, based on that, you will see that I decided to use CSS position properties instead of CSS grid or flex layout, why that? Well, how it's just an element on the entire body of the site, I thought that it would fit well, a simple way to put things into place, and how it's just one element, I don't need to worry about breaking the layout.

About the responsible part of the page, well, I didn't need to make any changes to the layout of the desktop version, cause the position properties already do the job to put the things in place based on view size.
</details>

### Updates after challenge
After I received some suggestions from the front-end mentor community, I decided to change some of my initial decisions to make it more responsible and improve the accessibility of my page.

First of all, I made the mistake of skipping one header level, so now it's corrected.

- before

  ```html
  <h2 class="card-title">Improve your front-end skills by building projects</h2>
  ```

- after

  ```html
  <h1 class="card-title">Improve your front-end skills by building projects</h1>
  ```

Then I added a tag _footer_ to wrap my attribution, with it my project will become better organized in code and to screen readers.

```html
<footer>
  <div class="attribution">
    <p>
      Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
      Coded by <a target="_blank" href="https://github.com/EvandeeMoS">EvandeeMoS</a>.
    </p>
  </div>
</footer>
```

On CSS, I've changed my decision of use _css position_ to use the _css grid layout_, last time I was thinking that using position would be a faster way of making this simple page with just one element, but after the suggestions, the grid layout proved to be more efficient even to this simple page.

```css
body {
  min-height: 100vh;

  display: grid;
  grid-template-rows: 100vh auto;
  place-items: center;

  background-color: #d6e2f0;
  font-family: 'Outfit', sans-serif;

  font-size: 1.5rem;
}
```

To finish it, I changed the units used in CSS to responsive ones, now it's responsive to the changes in browser base font-size changes. As you can see in these parts of the code for example:

- This is a tip that from a video, make the font-size base 10px instead of 16px so it's easier to think of sizes.
  ```css
  html {
      font-size: 0.625rem;
  }
  ```

- Base font-sized defined
  ```css
  body {
    font-size: 1.5rem;
  }
  ```

- Changed font-size to card titles
  
  ```css
  .card-title {
    margin: 1.6rem;
    font-size: 1.46em;
    color: #1f3251;
  }
  ```
## Author

- Frontend Mentor - [@EvandeeMoS](https://www.frontendmentor.io/profile/EvandeeMoS)

## Acknowledgments

Here are some fellows of frontend mentor that helped with their suggestions into comments on my solution:
[@Hassiai](https://www.frontendmentor.io/profile/Hassiai), [@ecemgo](https://www.frontendmentor.io/profile/ecemgo) and [@sumanth-chandana](https://www.frontendmentor.io/profile/sumanth-chandana)