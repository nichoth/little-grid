# Little Sass Grid #
Simple little responsive Sass grid with 12 columns.

## Install ##

```bash
$ bower install little-grid
```

## Use ##

```sass
// main.scss

// use my own variables
$siteMaxWidth: 1024px;
$littleGridNamespace: "lg-";

@import "bower_components/little-grid/little-grid"
```

## Variables ##
You can set these variables:

* $columns -- number of columns
* $siteMaxWidth -- width of the site. Used to calculate the row max width.
* $columnGutter -- size of the space between columns
* $littleGridNamespace -- a prefix to use on all class names

Markup Example:

```html
<!-- grid -->
<div class="wrapper">
    <div class="row">
        <div class="span6"> Six column div </div>
        <div class="span6 last"> Another six column div </div>
    </div>
</div>
```

Use `.row-uniform` when all columns are equal width

```html
<div class="wrapper">
    <div class="row-uniform">
        <div class="span6"> Six column div </div>
        <div class="span6"> Another six column div </div>
    </div>
</div>
```

Offset columns:

```html
<!-- offset columns -->
<div class="wrapper">
    <div class="row">
        <div class="span6 offset6 last">This spans columns 7 - 12</div>
    </div>
</div>
```

