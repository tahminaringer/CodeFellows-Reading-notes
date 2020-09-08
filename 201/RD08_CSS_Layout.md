# Read 08 - CSS Layout

- CSS treats each HTML element as if it is in its own box.
  - `Block level elements` Start on a new line
    - `<h1> <p> <ul> <li>`
  - `Inline Elements` flow in between surrounding text
    - `<img><b><i>`
- **Containing Elements** If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.
  - common to group a number of elements together inside a `<div>`

## Controlling the position of elements

- **Positioning Schemes** Allow you to control the layout of a page
  - *normal flow* every block-level element appears on a new line. default of browser.
  - *relative positioning* moves an element fromthe position it would be in normal flow, shifting it to the top, right, bottom or left of where it would have been placed
  - *absolute positioning* positions the element in relation to its containing element. Does not affect the postion of any surrounding elements
  - *Fixed positioning* absolute positioning that positions an element in relation to the browser window, as opped to the containing element. Do not move when scrolled
  - *floating elements* allows you to take that element out of normal flow and position it to the far left or right of a containing box. it becomes a block-level element arnd which other content can flow.
- **z-index** allows you to control which box appears on top.
- **Normal Flow** each block-level element sits on top of the next one.
  - `position:static`
- **Relative Positioning** moves an element in relation to where it would have been in normal flow.
  - `position:relative`
- **Absoluet positioning** when position property is given a value of absolute, the box is taken out of normal flow and no longer affects the position of other elements on the page.
  - `position:absolute`
- **Fixed Positioning** is a type of absolute positioning that requires the position property to have a value of fixed.
  - `position:fixed`
- **Overlapping Elements** when you use relative fixed or absoluet positioning, boxes can overlap. To control which element sits on top you can use **z-index**
  - `z-index`
- **Floating Elements** allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible.
  - `float`
  - commonly used to place boxes next to eachother
- **Clearing Floats** allows you to say that no element within the same containing element should touch the left or right handsides of a box
  - `left` 
  - `right`
  - `both`
  - `none`
- **Creating Multi-Column Layouts w/ floats**used to position the columns next to eachother
  - width
  - Margin
  - float
- **Screen Sizes** average webpage 960-1000px
- **Fixed width layout** don't change size as the user increases or decreases the size of their browser window.
  - uses pixels
- **Liquid Layouts** stretch and contract as the user increases or decreases the size of their browser window.
  - uses percentages
- **CSS Frameworks** make life easier by providing the code for common tasks such as creating layout grids styling forms, printer friendly versions of pages, etc.
