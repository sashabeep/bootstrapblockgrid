## Bootstrap 4 block grid

Tired of amount of classes you should apply to each column in bootatrap?

```html
<div class="container">
    <div class="row">
        <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3 col-lg-2">Col</div>
        <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3 col-lg-2">Col</div>
        <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3 col-lg-2">Col</div>
        <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3 col-lg-2">Col</div>
        <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3 col-lg-2">Col</div>
        <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3 col-lg-2">Col</div>
    </div>
</div>
```

### Dead simple solution!

Control number of columns by adding class to your **.row**

```html
<div class="container">
    <div class="row xs-up-1 sm-up-2 md-up-3 lg-up-4 xl-up-6">
        <div class="col">Col</div>
        <div class="col">Col</div>
        <div class="col">Col</div>
        <div class="col">Col</div>
        <div class="col">Col</div>
        <div class="col">Col</div>
    </div>
</div>
```
### DEMO
![](demo.gif)

### How to do this?

1. Include ```bootatrap-block.css``` from ```/dist/``` directory of this repository
2. Apply "up-to" classes to your row which define number of columns on particular breakpoint
3. That's it

### Every number from 1 to 12

5, 7, 11 columns in row? No problem!

### Customizing

By default, css is compiled with default bootstrap breakpoints.

```sass
$breakpoints:
(xs: 576px,
sm: 768px,
md: 992px,
lg: 1200px);
```

Feel free to change source SCSS from ```/src/``` directory of this repository.
Mixins for responsive breakpoints taken from https://glennmccomb.com/articles/useful-sass-scss-media-query-mixins-for-bootstrap/

### If it helps?

Donate a couple of bucks on [paypal](https://www.paypal.me/sashabeep) if you wanted.
