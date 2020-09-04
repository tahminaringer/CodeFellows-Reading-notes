# Reading 04- HTML Links, CSS Layout and JS Functions

## Chapter 4

- **Links** Links are created using an `<a>` `<a href="http://www.google.com">Google</a>`
- Directories are good to organize each different section of a larger site
- Relationships between the files and folders of the website are described as a family tree- grandparent, parent, child, grandchild, etc.
- **Relative URL** can be used to link between pages in site
- **Email Link** starts up user's email program and addresses email to specified email address
  - use `<a>` `href` attribute starts with `mailto:` and is follow by the email address you want the email sent to.
- **Opening links in new window** use target attribute within `<a>`
  - `<a href="http://www.google.com" target="_blank">Google</a>`
- **Linking to a Specific Part of same Page** 
  - Identify the points in the page that the link will go to by using `id attribute`

## HTML Chapter 15 - Layout

- **Block-level Boxes** start on a new line and act as the main building blocks of any layout
  - If a block-level sits inside a block-level outer box is known as parent.
- **inline boxes** flow between surrounding text
- it is common to group number of elements together within a `<div>`
- The element that contains group is known as the containing element
- **Layout Control** 
  - **normal flow** every block-level element appears on a new line
  - **relative positioning** moves an element to top right bottom or left
    - moves element to where it would have been in normal flow
  - **Absolute positioning** positions in relation to it's containing element
    - move as user scroll up and down the page
  - **fixed positioning** positions in relation to the browser window as apposed to the containing element
  - **floating elements** allows you to position in the far right or left of a containg box.
    - the floated element becomes a block-level element where content can not flow
    - can be used to place boxes next to eachother
    - **clear** allows you to say no element in container should touch the left or right had sides of the box
  - **z-index control** controls which element sits on top on one another. also known as `stacking content`
  - **Multiple Column Layouts** achieved by using a `<div>` to represent each column. 
    - `width`sets the width
    - `float` positions columns next to one another
    - `margin` creates gap between columns
- **page size** pages tend to be 960-1000px wide
  - **Fixed Width Layout** designs do not change size as user increases or decreases browswer size.
    - can use CSS to fix the `width: 960-1000px;`
  - **Liquid Layouts** stretch and contract as the user increases or decreases the browser size
  - uses percentages to specify the width `width: 90%;`
  - **Layout Grid** used to structure the elements appropieately on the page.
  - **CSS Frameworks** provide layout grids, styling forms, printer-frendly versions of pages etc.

## JS Chapter 3 Functions, Methods and Objects

- **Functions** let you group a series of statements together to perform a specific task
- functions let you group a series of statements to gether to perform a specific task
- if different parts of a scrpt repeat the same task you can reuse the function instead of repeating the same statment
- helps organize code
- stores steps needed to achieve a task
- calling the fuction is asking it to perform its task
- **parameters** pieces of information passed to a function
 - codevariable that defines a reference for an argument. defined within function.
- **return value** the expected answer to a function
- **Declaring the function**
  - `function sayHello() {`
      `document.write('hello');`
- **Calling a Function** asking function to perform
  - `sayHello();`
- **Declaring Functions that need Information**
  - `function getArea(width, height) {`
      `return width * height;`
- **Calling functions that need information**
  - **Argument** value that exists outside of the function signature
  - **Arguments as Values**`getArea(3, 5);`
  - **Arguments as Variables**
  `wallWidth = 3;`
  `wallHeight + 5;`
  `getArea(wallWidth, wallHeight);`
- **Function Delclaration** creates a function you can call later in code
  - must give it a name, also called *named function*
- **Local variable** When a variable is created inside a fuction using a var keyword
- **Global Variables** variable that can be used anywhere in script

## 6 Reasons for Pair Programming

- Driver and navigator - driver types code/navigator guides the executed code
- Why greater efficiency, easier to catch mistakes. 
- takes slightly longer but produces better quality
- can learn from eachother
- aid for improved communication
- job readiness
- Work environment readiness
