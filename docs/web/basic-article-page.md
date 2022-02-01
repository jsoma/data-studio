# Building a basic article template

While the examples on this page have the styles and html next to one another, the styles really belong in a stylesheet.

## Centering your text in a column

If you're using a CSS template you might get this automatically as part of the template. If not, the code below will create a 760px column in the middle of the page for your text. As a bonus, images inside of the text container will never grow outside of it, even if they're huge.

```html
<style>
    .text-container {
        max-width: 760px;
        margin: 0 auto;
    }
    .text-container img {
        max-width: 100%;
    }
</style>
<div class='text-container'>
    <p>Here is some long text</p>
    <img src="sample.jpg">
    <p>Here is some long text</p>
</div>
```

## Full-bleed headers and images

Using background images is a great way to stack text on top of images, and is a common way to do "hero" or header images.

Note that the CSS rules are about background size and position, while the actual image is specified inline, as `style='background-image: url("bg.jpg");'`. This allows you to use the `full-bleed-image` class anywhere, and each time specify the image you're like as the background.

```html
<style>
    .full-bleed-image {
        background-size: cover;
        background-position: center center;
    }

    .full-bleed-image .image-text {
        color: white;
        text-shadow: 0 0 20px black;
    }
</style>
<div class='full-bleed-image' style='background-image: url("bg.jpg")'>
    <div class='text-container'>
        <div class='image-text'>Here is some text</div>
    </div>
</div>
<div class='text-container'>
    <p>Here is some long text</p>
</div>
```

!!! danger "missing images"

When you use `background-image`, it always looks for the image in the same place you have the style. So if you moved it into the stylesheet, it would look for the image in the same directory as the stylesheet, *even if it's not in the same folder as `index.html`.

## Chart titles, subtitles, captions

Positioning your chart in a special `div` allows you to style a header, subhead and caption. You might need to add a `max-width: 100%` to the image if you didn't use the code from higher up on this page.

Be sure to add an `alt` tag for screen readers and general accessibility! Even if you have a descriptive subtitle you'll still need to do this.

```html
<style>
    .chart-holder h3 {
        font-weight: bold;
    }
    .chart-holder .subtitle {
        font-size: 1.2em;
    }
    .chart-holder .caption {
        font-size: 0.9;
        color: grey;
        text-align: right;
    }
</style>
<div class='text-container'>
    <p>Here is some long text</p>
    <div class='chart-holder'>
        <h3>Here is the title</h3>
        <div class='subtitle'>This is a subtitle</div>
        <img alt="Here is a description of the chart" src='plot.png'>
        <div class='caption'>Summary of the data source</div>
    </div>
</div>
```
