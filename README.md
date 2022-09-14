
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


```css
#styles.css

```
> **Step 11** <br>


```html
#index.html

```
> **Step 12** <br>


```html
#index.html

```
> **Step 13** <br>


```html
#index.html

```
> **Step 14** <br>


```html
#index.html

```
> **Step 15** <br>


```html
#index.html

```
> **Step 16** <br>


```css
#styles.css

```
> **Step 17** <br>


```css
#styles.css

```
> **Step 18** <br>


```css
#styles.css

```
> **Step 19** <br>


```css
#styles.css

```
> **Step 20** <br>


```css
#styles.css

```
> **Step 21** <br>


```css
#styles.css

```
> **Step 22** <br>


```css
#styles.css

```
> **Step 23** <br>


```css
#styles.css

```
> **Step 24** <br>


```css
#styles.css

```
> **Step 25** <br>


```css
#styles.css

```
> **Step 26** <br>


```css
#styles.css

```
> **Step 27** <br>


```css
#styles.css

```
> **Step 28** <br>


```css
#styles.css

```
> **Step 29** <br>


```css
#styles.css

```
> **Step 30** <br>


```css
#styles.css

```
> **Step 31** <br>


```css
#styles.css

```
> **Step 32** <br>


```css
#styles.css

```
> **Step 33** <br>


```css
#styles.css

```