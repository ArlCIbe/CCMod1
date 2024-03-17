##### Every HTML element has a default **display** value, which controls how it shows up on a WP. The default display is usually **block** or **inline**, which is dependent on the browser's **normal flow** (how it lays out HTML pages by default). The methods that can change how elements are laid out in CSS are:

#### Block-level - starts on a new line and takes up the full width available (stretches out to the left and right as far as possible).

- ###### flex - creates a block-level flex container
- ###### grid - creates a block-level grid container

#### Inline - doesn't start on a new line and only takes up as much width as necessary.

- ###### inline-flex - creates an inline-level flex container
- ###### inline-grid - creates an inline-level grid container
- ###### inline-table - creates an inline-level table

##### inline-block - creates an inline-level block container; the element itself is formatted as an inline element, but you can apply height and width values.

#### other display property values

- contents - makes the container disappear, making the child elements children of the element the next level up in the DOM
- list-item - lets the element behave like a <li> element
- run-in - displays an element as either block or inline, depending on contex
- table - lets the element behave like a <table> element
- table-caption - lets the element behave like a <caption> element
- table-column-group - lets the element behave like a <colgroup> element
- table-header-group - lets the element behave like a <thead> element
- table-footer-group - lets the element behave like a <tfoot> element
- table-row-group - lets the element behave like a <tbody> element
- table-cell - lets the element behave like a <td> element
- table-column - lets the element behave like a <col> element
- table-row - lets the element behave like a <tr> element
- none - the element is completely removed
- initial - sets this property to its default value
- inherit - inherits this property from its parent element

___

### NONE

- commonly used with JavaScript to hide and show elements without deleting and recreating them
G2K: `script` defaults to display: none.

**Note**: Setting the display property of an element only changes *how* the element is displayed, not what *kind* of element it is (e.g. an inline element with display: block; is not allowed to have other block elements inside it).

#### Hiding an Element

**display: none** - the page will be display as if the element is simply not there. 
**visibility:hidden** - b/c it's still taking up the same space as before, the element will affect the page layout.

### FLEX

- applying **display: flex** to an element causes all of that element's *DIRECT* children to become flex items, meaning they'll be affected by some of the **initial** values that flexbox sets on the flex container

- In addition to properties that can be applied to a flex *container*, there are also properties that can be applied to flex *items*, enabling them to expand or contract according to available space.
    - **flex: 1** will cause all of these flex *items* to fill the container insead of leaving space at the end

### GRID

- ##### grid-template-rows
- ##### grid-template-columns




