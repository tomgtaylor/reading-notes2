# Class 08 - More CSS Layout

CSS Flexbox

> The Flexible Box Layout Model (flexbox) is a layout model designed for one-dimensional content. It excels at taking a bunch of items which have different sizes, and returning the best layout for those items.  - web.dev 


One can use a flex layout to do the following:

- display a row or column.
- single line, but can be asked to wrap onto multiple lines.
- items in layout can be visually reordered away from their order
- space can be distrubuted inside and around the items.

Terms used in CSS - Flexbox:

    row: the items lay out as a row.
    row-reverse: the items lay out as a row from the end of the flex container.
    column: the items lay out as a column.
    column-reverse : the items lay out as a column from the end of the flex container.

Example of creating a flex box/container

    <div class="container" id="container">
      <div>One</div>
      <div>Item two</div>
      <div>The item we will refer to as three</div>
    </div>

To use flexbox you need to declare that you want to use a flex formatting context and not regular block and inline layout. Do this by changing the value of the display property to flex.

    .container {
      display: flex;
    }

---

CSS Layout - 

## Things I want to know more about

- More about how actually use flexbox
- Practical usage

[Previous Page](https://tomgtaylor.github.io/reading-notes2/class-07)    ||    [Next Page](https://tomgtaylor.github.io/reading-notes2/class-09) <br>

---
[HOME](https://tomgtaylor.github.io/reading-notes2) <br>
