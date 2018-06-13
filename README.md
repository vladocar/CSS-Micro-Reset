# CSS Micro Reset

You probably don't need CSS Reset, at least not complete CSS Reset.

Every Browser has it's own CSS Reset. Reseting it again means that later you need to set all reseted elements.

Basically you have Browser Reset -> Your Reset ->  Setting all Reseted Elements -> probably another styling at the end.

#### Let take typical H1 tag mistake:

```css
/* Chrome  Reset */

h1 {
    display: block;
    font-size: 2em;
    -webkit-margin-before: 0.67em;
    -webkit-margin-after: 0.67em;
    -webkit-margin-start: 0px;
    -webkit-margin-end: 0px;
    font-weight: bold;
}

/* Your Reset */

h1 {
  margin: 0;
  padding: 0;
  border: 0;
  line-height: 1;
  font-weight: normal;

}

/* Now you need to set the H1 */

h1 {
  margin: 0 0 0 1em;
  line-height: 1.5;
  font-weight: normal;
}

/* And probably you will do one more H1 setting */

h1 {
color: #111;
font: 2em/1.5 Arial, sans-serif;
font-weight: normal;
}

/* I will assume one or two more setting of H1 tag here :) */
```
**We all did this mistake too many times.**

Why not skip the reset and set just the elements you need for your project?

Also why reseting some elements if you are not using them in your project. Example: If you don't have forms in your project don't reset them.

Other thing: It's Ok some elements to be different in different browsers.

Why not start with bare bones reset and if needed add some elements?

I've did just that: **Micro CSS Reset**

Feel free to add  or remove elements to Micro CSS Reset, don't just blindly use it. Example: if don't use tables remove all the table related tags in the Micro CSS Reset.

Like I said in the beginning: You may not need this or any other CSS reset.

*Before use, understand what this reset does.*

## Download or Install

You can copy-paste the CSS code, use direct download, or use npm:

```
$ npm i css-micro-reset
```
Or use the CDN link:

```html
 <link rel="stylesheet" href="https://unpkg.com/css-micro-reset@1.0.0/micro-css-reset.css">
 ```

### License

This project is licensed under the MIT License
