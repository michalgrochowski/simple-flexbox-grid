# Simple Flexbox Grid

## So, this is a very simple Flexbox based grid system with 12 columns.

###### 1. Configuration

You can find everything in `_variables.scss` file:
- Colors - basic colors, not relevant to the grid,
- Grid values - here you can set your container width, columns gutter and row padding,
- Media breakpoints - main thing - breakpoints values used in the grid system,
- Grid size - container width divided by 12 minus gutters,
- Offsets - container width divided by 12 plus gutters.

###### 2. Basic usage

First of all, your main container should have a class of `grid`, which is set to `1200px`, but you can change that in cofniguration file. Then add as many rows as you like inside it and start building your website. You can also nest rows, doing something like this - `grid -> row -> column -> another row -> column -> another row` etc.

###### 3. Columns

If you ever used Bootstrap you should see some resemblance (yeah, "some"...) - you use classes like `col-xs-[value]` in your rows blocks and chain them for different sizes, so for example `<div class="col-xs-12 col-col-sm-12 col-md-6 col-lg-4 col-xl-2">WoW</div>`. If you have more than 12 columns in a row they will start stacking on a new line, so remember that your block should always add to 12.

###### 4. Offsets

Like in Bootstrap, you can offset your columns using `col-[size]-offset-[value]` - it will add a margin-left to your column which will push it, so you can have for example a 4/12 column, 4/12 gap and another 4/12 column using `<div class="col-xs-offset-4 col-xs-4"`.


#### So there you go, a simple grid, built with Flexbox and SCSS.


##### Demo: https://michalgrochowski.github.io/simple-flexbox-grid/dist/

License: MIT
