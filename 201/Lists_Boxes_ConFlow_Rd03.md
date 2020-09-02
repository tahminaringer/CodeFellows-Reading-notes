# Reading 03- HTML Lists, CSS Boxes, JS Control Flow

## Chapter 3 Lists

- `<ol>` Ordered lists
  - `<li>` Stands for list item
  - *Nested Lists* you can put a second list inside of `<li>`
- `<ul>` Unorded list
- `<dl>` definition list
  - `<dt>`contains the term being defined
  - `<dd>` Used to contain the definition

## Chapter 13 Boxes

- **Box Dimensions** use `height` and `width` properties to set box size, otherwise will be set to fit content
  - when you use percentages the size of the box is set to the size of browzer window
  - when use ems the size of the box is based on the size of text within it
- **limiting width** use `min-width`, `max-width`helps content change size to appropriately fit different screen sizes
  - makes sure content of page is ledgable
- **Limiting height** `min-height` `max-height`
- **Overflow** tells browser what to do if the content contained within a boc is larger than the box itself
 - *hidden* this property hides excess content
 - *scroll* adds a scroll bar to box
- **Border** separates the edge of one box from another
- **Margin** creates gaps between the borders of two adjacent boxes
- **Padding** space between the border of a box and any content contained with in it.
- **White space** Space between items on page
- **Border-width** Controls the of a border- thin med thick or in pixels
- **Border-Style** controls style of border- solid, dotted, dashed, double, groove, ridge, inset, outset, hidden
- **Border-color** specifies the color of border
-**Short hand**
 ``p{`
      `width: 250px;`
      `border: 3px dotted color;`
  `}`
- **Centering Content** set `left-margin` `right-margin` to auto
  - must set a with for the box or it will take up full page
- **Display element** turns an inline element into a block-level elelment or vice versa can also hide element
  - `inline` causes a block-level element to act like an inline elelment
  - `inline-block` causes block-level element to flow like an inline element
  - `none` hides an element from the page
- **Visibility**  allows you to hid boxes from users but leaves space where it would have been
  - `hidden` hides element
  - `visible` shows element
- **border image** applies an image to the border of any box- requires 3 pieces of info
  1. The URL of image
  2. Where to slice the image
  3. What to do with the straight edges
    - stretch- stretches image
    - repeat- repeats image
    - round- scales the tile image so it fits
- **Box Shadows** allows you to add a drop shadow around box
  - horizontal offset
  - vertical offset
  - blur distance
  - spread of shadow
- **border-radius** creates rounded corners on box

## JS Chapter 3 

- **Arrays** variable that stores a list of variables
  - use when working iwht a list or set of values related to eachother
  - great if you dont know how many items a list will contain
  `var colors;`
  `colors = ['white', 'green', 'yellow'];`
- **Values in Arrays** accessed if they are in a numbered list. Numbering starts at 0
  - *index* number given to each item in an array
  - array name is specified along with the idex number in `[]`
  -*length* is the property wich holds the number of items in an array

## JS Chapter 4

- **If...Else Statements** checks a condition, if true the first codebock is exicuted, if false the second codeblock is run
- **Switch statements** Start with a variable called switch value, each case indicates a possible value the variable and the code that should run if match
- **type coercion** when JS converts data types behind the scenes to complete operation
- **Falsy** treated as if they are false
- **Truthy** treated as if they are true
- **Unary operator** returns a result with just one operand
- **Loops**Check a condition, if true, a code block will run. repeats
  - **For** if need to run for specific amount of times use **for** loop
    - ex: password- after entering wrong x amount times get blocked
  - **While** if amount of times unknown. loops as long as condition is true
  - continue to loop when user answers false, until user enter an answer that is true, runs until user answer is once again false. true and false interchangable- Password senario.
  - **Do While** similar to *while* loop but will always run the statements inside the curly brac es atleast 1 even if statement is false
  -**Initializeation** *i* Create a variable and set it to 0
  - **Condition** will run until reaches a specific number
  - **Update** Everytime loop runs it add one to the counter
  - **Break** causes termination of loop
  - **continue** tells interpreter to stop, update and check the condition
  -**infinite loop** Code will not stop running until browser runs out of memeory and breaks code
