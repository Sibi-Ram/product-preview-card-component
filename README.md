 # Product Preview Card Component

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### Screenshot

#### Desktop view:
![Desktop view](./screenshots/desktop-view.jpg)

#### Modile view:
![Mobile view](./screenshots/mobile-view.jpg)

### Links

- Source Code: [view on GitHub](https://github.com/Sibi-Ram/product-preview-card-component)
- Live Site URL: [Product Preview Card Component website](https://sibi-ram.github.io/product-preview-card-component/)

## My process

### Built with


- ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
- ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
- Flexbox

### What I learned

#### **<s>StrikeThrough</s>:**

I learned to use ```<s>``` tag to display text with a strikethrough, which can also be used within the ```<p>``` tag

```html
<s>StrikeThrough Text</s>
```
#### **<u>Nth-child and nth-of-type pseudo-classes</u>**

- :nth-child(n) selects the nᵗʰ child of its parent, counting all element types.
    
- :nth-of-type(n) selects the nᵗʰ child among siblings of the same tag name.

  - Counting Context

       - nth-child: counts every child regardless of tag.
      - nth-of-type: counts only children matching the element’s tag.

    - ">" is child combinator

```css
position-based pseudo-classes.
  .description-container > p:nth-child(1){
    letter-spacing: 0.3125rem;
    color: #6C7289;
  }
  
  
  .description-container > p:nth-of-type(2){
    color: #6C7289;
    line-height: 1.6;
    font-size: 0.875rem;
  }
  
  

```


### <u>IMAGE</u>
#### Image(icon) within the Button

  Inside a ```<button>``` tag, I can include a variety of HTML content such as

  - Plain text
  - Images or icons ( ```<img>``` tag)
  - Inline elements like ```<span>, <i>, <b>, <strong>, <em>```
       

  ```html
<button type="button">
 <img src="./images/icon-cart.svg" alt="cart-icon" >
      Add to Cart</button>
  ```

  Can Alter the size of image inside button in CSS also used Flex-box to center and align the image icon and text inside button


#### **picture**

```<picture>``` helps me to provide different image based ont he device width- one for mobile device one for desktop

```html
<picture class="img-container">

<!-- Desktop full image -->
    <source srcset="./images/image-product-desktop.jpg" media="(min-width: 37.5rem)">
<!-- Mobile crop -->
    <source srcset="./images/image-product-mobile.jpg" media="(max-width: 37.4rem)">

    <img src="./images/image-product-mobile.jpg" alt="Perfume bottle with elegant glass design" loading="lazy">
  </picture>
```
can also use ```<picture>``` for different image format

```loading="lazy"``` attribute on the ```<img> ```element inside a ```<picture>``` element is used to *defer* loading the image until it is about to enter the *user’s viewport*. Image is not loaded immediately when the page loads, but only based on viewport width.

#### **overflow**

```css
.container{
  overflow: hidden;
}
```
It Hides the excess cotnent that extends outside of a container’s borders

#### flex:1
```css
flex:1;
```

```flex: 1``` on flex children makes them take equal width sharing the ***container space evenly 50%***.










**Key Learning:**

___Picture element can be used to change the image based on device width, also can use multiple formats and can use fallback image___


## Author

- Twitter - [SRtheDev](https://www.twitter.com/SRtheDev)
- Frontend Mentor - [Sibi-Ram](https://www.frontendmentor.io/profile/Sibi-Ram)



## Acknowledgments

This is my solution to the [Preview card Component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa).

