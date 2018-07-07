# Juiceboxes/juice-grid

A very lightweight grid system using CSS Grid.

This is not a complete grid, but, like other juicebox repos, is a lightweight product used for rapid prototyping.

## Installing
`npm install @juiceboxes/juice-grid`

### Imports
Regular CSS: `@import 'node_modules/@juiceboxes/juice-grid/juice-grid.css'`

Minified CSS: `@import 'node_modules/@juiceboxes/juice-grid/juice-grid.min.css'`

SCSS with Variable declarations: `@import 'node_modules/@juiceboxes/juice-grid/juice-grid.scss'`

## Useage

### Basic
``` html
<div class="jb-grid">
    <div class="jb-row">
        <div class="jb-col-4">4 Columns</div>
        <div class="jb-col-8">8 Columns</div>
    </div>
</div>
```

### With Gutters

Before your import of the `.scss` file, declare your `$jb-grid_gutter` variable. Otherwise, the default is `15px`.

``` html
<div class="jb-grid with-gutters">
    .
    .
    .
</div>
```

### Offsetting Columns
``` html
<div class="jb-grid">
    <div class="jb-row">
        <div class="jb-col-4 jb-push-8">4 Column span starting at column 9 (spans col 9, 10 ,11 ,12)</div>
    </div>
</div>
```

## Development
`npm run start` will build and watch the `index.pug` and `src/juice-grid.scss` files