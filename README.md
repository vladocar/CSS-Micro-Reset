# CSS Micro Reset

You probably don't need CSS Reset, at least not the complete CSS Reset.

Every Browser has its own CSS Reset. Resetting it again means that later you need to set all reset elements.

Basically you have:

Browser Reset -> Your Reset ->  Setting all Reset Elements -> Probably more styling after.

#### A typical `H1` tag mistake:

```css
/* "Chrome  Reset" - default Chrome CSS stylesheet */

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

/* And probably you will do one more further H1 setting */

h1 {
color: #111;
font: 2em/1.5 Arial, sans-serif;
font-weight: normal;
}

/* I will assume one or two more setting of H1 tag here :) */
```

#### We've all made this mistake too many times.

Why not skip the reset and just set the elements that you need for your project?

Also why are you resetting some elements if you are not using them in your project. For example, if you don't have forms in your project, don't reset them.

Another thing: It's Ok for some elements to be different between browsers.

Why not start with bare bones reset and only add some elements if needed?

I've done just that: **CSS Micro Reset**

Feel free to add or remove elements to CSS Micro Reset, don't just blindly use it. For example, if you don't use tables, remove all the table related tags in the CSS Micro Reset.

Like I said in the beginning: You may not need this or any other CSS reset.

*Before use, understand what this reset does.*

## Download or Install

You can copy-paste the CSS code, use the direct download, or use npm:

*Note: I'm avere that using npm for project this small is ridiculous. But when I don't put npm there is always someone who complains why there is no: npm, yarn, bower and where is CDN link?*

```
$ npm i css-micro-reset
```
Or use the CDN link:

```html
 <link rel="stylesheet" href="https://unpkg.com/css-micro-reset@1.0.0/micro-css-reset.css">
 ```

## License

This project is licensed under the MIT License
