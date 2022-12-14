
# Learn Responsive Web Design by Building a Piano, Completed

> - Responsive Design tells your webpage how it should look on different-sized screens.
> - In this course, you'll use CSS and Responsive Design to code a piano. You'll also learn more about media queries and pseudo selectors.
---

> **Step 1** <br>
Begin with the basic HTML structure. Add a `DOCTYPE` declaration and `html`, `head`, `body`, and `title` elements.<br>
Set the language of this page to English. Set the `title` to `Piano`.

```html
#index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Piano</title>
  </head>
  <body></body>
</html>
```
> **Step 2** <br>
Add two `meta` tags, one to optimize your page for mobile devices, and one to specify an accepted `charset` for the page.

```html
#index.html
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
```
> **Step 3** <br>
Time to start working on the piano. Create a `div` element within your `body` element with the id set to `piano`.

```html
#index.html
    <div id="piano">
```
> **Step 4** <br>
Nest a second `div` within your existing `div`, and set the `class` to be `keys`.

```html
#index.html
    <div id="piano">
      <div class="keys"></div>
    </div>
```
> **Step 5** <br>
Within your `.keys` element, add seven `div` elements. Give them all the class `key`.

```html
#index.html
    <div id="piano">
      <div class="keys">
        <div class="key"></div>
        <div class="key"></div>
        <div class="key"></div>
        <div class="key"></div>
        <div class="key"></div>
        <div class="key"></div>
        <div class="key"></div>
      </div>
    </div>
```
> **Step 6** <br>
Remember that a `class` attribute can have multiple values. To separate your white keys from your black keys, you'll add a second `class` value of `black--key`. Add this to your second, third, fifth, sixth, and seventh `.key` elements.

```html
#index.html
    <div id="piano">
      <div class="keys">
        <div class="key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
        <div class="key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
      </div>
    </div>
```
> **Step 7** <br>
Now copy the set of seven `.key` elements, and paste two more sets into the `.keys` div.

```html
#index.html
    <div id="piano">
      <div class="keys">
        <div class="key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
        <div class="key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>

        <div class="key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
        <div class="key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>

        <div class="key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
        <div class="key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
      </div>
    </div>
```
> **Step 8** <br>
Add a `link` element within your `head` element. For that `link` element, set the `rel` attribute to `stylesheet` and the `href` to `./styles.css`.

```html
#index.html
    <link rel="stylesheet" href="./styles.css" />
```
> **Step 9** <br>
Browsers can apply default margin and padding values to specific elements. To make sure your piano looks correct, you need to reset the box model.<br>
Add an `html` rule selector to your CSS file, and set the `box-sizing` property to `border-box`.

```css
#styles.css
html {
  box-sizing: border-box;
}
```
> **Step 10** <br>
Now that you have reset the `html` box model, you need to pass that on to the elements within as well. To do this, you can set the `box-sizing` property to `inherit`, which will tell the targeted elements to use the same value as the parent element.<br>
You will also need to target the pseudo-elements, which are special keywords that follow a selector. The two pseudo-elements you will be using are the `::before` and `::after` pseudo-elements.<br>
The `::before` selector creates a pseudo-element which is the first child of the selected element, while the `::after` selector creates a pseudo-element which is the last child of the selected element. These pseudo-elements are often used to create cosmetic content, which you will see later in this project.<br>
For now, create a CSS selector to target all elements with `*`, and include the pseudo-elements with `::before` and `::after`. Set the `box-sizing` property to `inherit`.

```css
#styles.css
*, *::before, *::after {
  box-sizing: inherit;
}
```
> **Step 11** <br>
Now target your `#piano` element with an `id` selector. Set `background-color` property to `#00471b`, the `width` property to `992px` and the `height` property to `290px`.

```css
#styles.css
#piano {
  background-color: #00471b;
  width: 992px;
  height: 290px;
}
```
> **Step 12** <br>
Set the `margin` of the `#piano` to `80px auto`.

```css
#styles.css
#piano {
  background-color: #00471b;
  width: 992px;
  height: 290px;
  margin: 80px auto;
}
```
> **Step 13** <br>
Time to style the keys. Below the `#piano` rule, target the `.keys` element with a `class` selector. Give the new rule a `background-color` property of `#040404`, a `width` property of `949px` and a `height` property of `180px`.

```css
#styles.css
.keys {
  background-color: #040404;
  width: 949px;
  height: 180px;
}
```
> **Step 14** <br>
Give the `.keys` a `padding-left` of `2px`.

```css
#styles.css
.keys {
  background-color: #040404;
  width: 949px;
  height: 180px;
  padding-left: 2px;
}
```
> **Step 15** <br>
Move the keys into position by adjusting the `#piano` selector. Set the `padding` property to `90px 20px 0 20px`.

```css
#styles.css
#piano {
  background-color: #00471b;
  width: 992px;
  height: 290px;
  margin: 80px auto;
  padding: 90px 20px 0 20px;
}
```
> **Step 16** <br>
Time to style the keys themselves. Create a `class` selector for the `.key` elements. Set the `background-color` set to the value `#ffffff`, the `position` property to `relative`, the `width` property to `41px`, and the `height` property to `175px`.

```css
#styles.css
.key {
  background-color: #ffffff;
  position: relative;
  width: 41px;
  height: 175px;
}
```
> **Step 17** <br>
Give the `.key` a `margin` of `2px` and a `float` property set to `left`.

```css
#styles.css
.key {
  background-color: #ffffff;
  position: relative;
  width: 41px;
  height: 175px;
  margin: 2px;
  float: left;
}
```
> **Step 18** <br>
Now it is time to use the pseudo-selectors you prepared for earlier. To create the black keys, add a new `.key.black--key::after` selector. This will target the elements with the class `key black--key`, and select the pseudo-element after these elements in the HTML.<br>
In the new selector, set the `background-color` to `#1d1e22`. Also set the `content` property to `""`. This will make the pseudo-elements empty.<br>
The `content` property is used to set or override the content of the element. By default, the pseudo-elements created by the `::before` and `::after` pseudo-selectors are empty, and the elements will not be rendered to the page. Setting the `content` property to an empty string `""` will ensure the element is rendered to the page while still being empty.<br>
If you would like to experiment, try removing the `background-color` property and setting different values for the `content` property, such as `"???"`. Remember to undo these changes when you are done so the tests pass.

```css
#styles.css
.key.black--key::after {
  background-color: #1d1e22;
  content: "";
}
```
> **Step 19** <br>
Give the `.key.black--key::after` a `position` property set to `absolute` and a `left` property set to `-18px`.

```css
#styles.css
.key.black--key::after {
  background-color: #1d1e22;
  content: "";
  position: absolute;
  left: -18px;
}
```
> **Step 20** <br>
For the `.key.black--key::after`, set the `width` to `32px` and the `height` to `100px`.

```css
#styles.css
.key.black--key::after {
  background-color: #1d1e22;
  content: "";
  position: absolute;
  left: -18px;
  width: 32px;
  height: 100px;
}
```
> **Step 21** <br>
The piano needs the freeCodeCamp logo to make it official.<br>
Add an `img` element before your `.keys` element. Give the `img` a `class` of `logo`, and set the `src` to `https://cdn.freecodecamp.org/platform/universal/fcc_primary.svg`. Give it an `alt` text of `freeCodeCamp Logo`.

```html
#index.html
    <div id="piano">
      <img class="logo" src="https://cdn.freecodecamp.org/platform/universal/fcc_primary.svg" alt="freeCodeCamp Logo" />
      <div class="keys">
```
> **Step 22** <br>
Start styling the logo by creating a `.logo` selector. Set the `width` to `200px`, a `position` of `absolute` and a `top` set to `23px`.

```css
#styles.css
.logo {
  width: 200px;
  position: absolute;
  top: 23px;
}
```
> **Step 23** <br>
The `img` element needs its parent to have a `position` set as a point of reference. Set the `position` of the `#piano` selector to `relative`.

```css
#styles.css
#piano {
  background-color: #00471b;
  width: 992px;
  height: 290px;
  margin: 80px auto;
  padding: 90px 20px 0 20px;
  position: relative;
}
```
> **Step 24** <br>
To smooth the sharp edges of the piano and keys, start by giving the `#piano` a `border-radius` of `10px`.

```css
#styles.css
#piano {
  background-color: #00471b;
  width: 992px;
  height: 290px;
  margin: 80px auto;
  padding: 90px 20px 0 20px;
  position: relative;
  border-radius: 10px;
}
```
> **Step 25** <br>
Give the `.key` selector a `border-radius` value of `0 0 3px 3px`.

```css
#styles.css
.key {
  background-color: #ffffff;
  position: relative;
  width: 41px;
  height: 175px;
  margin: 2px;
  float: left;
  border-radius: 0 0 3px 3px;
}
```
> **Step 26** <br>
Give the `.key.black--key::after` selector a `border-radius` of `0 0 3px 3px` to match the keys.

```css
#styles.css
.key.black--key::after {
  background-color: #1d1e22;
  content: "";
  position: absolute;
  left: -18px;
  width: 32px;
  height: 100px;
  border-radius: 0 0 3px 3px;
}
```
> **Step 27** <br>
The `@media` at-rule, also known as a media query, is used to conditionally apply CSS. Media queries are commonly used to apply CSS based on the viewport width using the `max-width` and `min-width` properties.<br>
In the below example the padding is applied to the `.card` class when the viewport is `960px` wide and below.
> ```css
> #styles.css
> @media (max-width: 960px) {
>   .card {
>     padding: 2rem;
>   }
> }
> ```
> Add a media query that will be applied when the viewport is `768px` wide and below.

```css
#styles.css
@media (max-width: 768px) {

}
```
> **Step 28** <br>
Add a new `#piano` selector within your `@media` query, and set the `width` to `358px`.

```css
#styles.css
@media (max-width: 768px) {
  #piano {
    width: 358px;
  }
}
```
> **Step 29** <br>
Within the `@media` query, add a `.keys` selector and set the `width` to `318px`.

```css
#styles.css
@media (max-width: 768px) {
  #piano {
    width: 358px;
  }

  .keys {
    width: 318px;
  }
}
```
> **Step 30** <br>
Now add a `.logo` selector to the `@media` query, and set the `width` property to `150px`.

```css
#styles.css
@media (max-width: 768px) {
  #piano {
    width: 358px;
  }

  .keys {
    width: 318px;
  }

  .logo {
    width: 150px;
  }
}
```
> **Step 31** <br>
You might have noticed the keys collapse when the browser window is smaller than `768px`. Set `overflow` to `hidden` in the first `.keys` selector, to take care of this issue. This property will hide any element that is pushed outside the set `width` value of `.keys`.

```css
#styles.css
.keys {
  background-color: #040404;
  width: 949px;
  height: 180px;
  padding-left: 2px;
  overflow: hidden;
}
```
> **Step 32** <br>
Add another `@media` rule to apply if the browser window is bigger than `769px` but smaller than `1199px`.

```css
#styles.css
@media (min-width: 769px) and (max-width: 1199px) {

}
```
> **Step 33** <br>
For the new `@media` rule, set the `width` of the `#piano` to `675px` and the `width` of the `.keys` to `633px`.<br><br>
With that, your piano is complete!

```css
#styles.css
@media (max-width: 1199px) and (min-width: 769px) {
  #piano {
    width: 675px;
  }

  .keys {
    width: 633px;
  }
}
```