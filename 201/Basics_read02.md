# Read02- Basics of HTML, CSS & JS

## HTML/CSS Chapter 2

- **Structural Markup** used to describe headings and paragraphs
- **Semantic markup** provides extra emphasis like where emphasis is placed in a sentence.
- **headings** six levels of headings. h1-h6
  - `<H1>` is used for mainheadings
  - `<h2>` Subheadings
  - `<h3-6>`further sections under subheadings
- `<p>` creats paragraph
- `<b> <i>` enclosing words in these tags make them bold or italic
- `<sup>` contains characters that should be superscript/ suffixes of dates or mathmatical concepts.
    -used with foot notes or chemical formulas.
- **White Space** when browser comes across blank spaces or or lines in code it acts like they do not exist.
- `<br />` line break tag
- `<hr />` creates a break between themes similar to `________________________`
- **Visual Editors** resemble wordprocessors
  - *code views* shows code created by the visual editor
- **Sematic Markup** don't affect the structure of the page but add extra info
- `<em>`indicates where emphasis should be placed on selected words
  - browsers show in italics
- `<blockquote>` indicates that a block of text is a quotation
  - Used for long quotes that take up a whole page
- `<strong>` indicates elements content has strong importance
  - browsers show strong elements in bold
  - `<q>`used for shorter quotes
- `<abbr>` used for abbreviations or an acronym
- `<cite>` to referrence your a piece of work like book, paper, film etc
- `<dfn>` indicates the defining instance of a new term/ some browsers show in italics
- `<address>`contains contact details for the author of the page
- `<ins>` shows content that has been inserted into document
- `<del>` shows content that hs been deleted from document
- `<s>` indicates something that is no longer relevent but shouldn't be deleted

## HTML/CSS Chapter 10

- **Selectors** Indicate which element the rule applies to.
- **Declarations** Indicate how the elements referred to in the sector should be styled
- **Properties**  Indicate the aspects of the element your want to change
- **Values** Specify the settings you want to use for the chosen properties
- **`<link>`** used in HTML to tell where to find css file, uses three attributes
  - **href** path to CSS file
  - **type** type of document being linked to
  - **rel** relationship between HTML and file it is linked to
- **`<style>`** sits inside the `<head>` include CSS stles in HTML
  - uses the type attribute with a value of text/css
- **CSS Sectors** case sensitive- target rules to specific elements
- `!important` can be added after property to show most improtant
- **Selectors**
  - *Universal Selector* Targets all elements on the page
  - *Type Selector* Matches element names
  - *Class Selector* matches element's class value `.note {}`
  - *ID Selector* matches value of of ID attribute `#introduction{}`
  - *Child Selector* matches an element that is a direct child of another `li>a{}`
  - *Adjacent Sibling Selector* Matches an element that is the next sibling of another `h1+p {}`
  - *General Sibling Selector* Matches element of a sibling of another `h1~p{}`

## JS Chapter 2

- **Statement** individual steps that a computer follows
- REMEMBER- JS is case sensitive
- **Comments** Explain what code does `//comment`
- **variables** are used to prpresent values in your scripts that are likely to change
- To use variable need to declare you want to use it.
- **var** is keyword for variable
  - In order to use must give *var* a name or identifier
  - *declaring the variable* creating a variable and giving it a name
- **camelCase** variable more than one word first letter is lowercase all words after first letter is uppercase
- **Numerical Data Type** - used for counting/calulating sums
- **String Data Type** - versitile/add new content to a page and can include HTML markup
-**Boolean Data Type** like a switch either on or off can only have a value of true or false
- Once you have asigned the value of a vaiable you can change what is stored in the variable later.
- once variable is created you can do away with the *var* `var inStock` to `inStock`

### Rules for Naming Variables

1. name always begins with `letter $ or _` never starts with number
2. can contain `letters, numbers, $ or _` never use `- or .`
3. Don't use keywords or reserved words such as `var`
4. All variable are case sensitive score and Score different variables
5. Use a name that is a descriptor of information stored
6. if more than one word use camelCase

- **Arrays** store a list of values
  - Use when working with a list or set of values that are related
  - Don't need to be the same data type can be a mix of string, number, boolean etc
- **Values in Arrays** values are accesed like in a numbered list that starts at 0
  - Each array is automatically given a number called and **index**
- **Expressions** Two types
  - expressions that just asign value to a variable `var color = 'green';`
  - expressions that uses 2 or more values to return a single value `var area = 3 * 2;`
  - **Operators** allow programers to create a single value from mor values
    - *Assignment opperators* Assign a value to a vaiable
    - *Arithmetic Operators* Perform basic math
      - Addition `+`
      - Subtraction `-`
      - Division `/`
      - Multiplication `*`
      - Increment `++`
      - Decrement `--`
      - Modulus `%`
    - *String Oporators* Combine 2 strings
    - *Comparison Oporators* Compare 2 ovalues and return true or false
    - *Logical Oporators* Combine expressions and return true or false

### Comparison Operators

- comparison operators generally return values of true or false. Logical operators allow you to compare the results of more than one comparison operator.
- `==`-equal to - compares two values
- `!=` - is not equal to-compares two values(numbers, strings, booleans) to see if they are **NOT** the same
- `===` -strict equal- compares two values to check that both the data type and value are the same
- `!==`-Strict not equal- compares two values to check that both the data type and value are **not** the same.
- `>` - greater than
- `<` - less than
- `>=`- greather than or = to
- `<=`- less than or = to
- **Operand** can be an expression or a single value or variable name
- comparison operators generally return values of true or false. Logical operators allow you to compare the results of more than one comparison operator.
- logical opperator checks to see if both expressions are true
- `**&&**` This oporator tests more than one condition. `((2<5) && (3>=2))`
- `**||**` test at least one condition. if either expression returns true then expression returns true `((2<5) || (2<1))`.
- `**!**` This operator takes a single boolean value and inverts it.`!(2<1)`
- **If Statements** evaluates a condition, if true, all statements in codeblock are executed. If false codeblock is not run

## Git Message

- Well crafted message is the best way to relay changes to developer team and for future edits
- **7 Rules of  a great git message**
  1. Separate subject from body with a blank line
  2. Limit the subject line to 50 characters
  3. Capatalize the subject line
  4. Do not end the subject line with a period
  6. Wrap the body a 72 characters
  7. Use the body to explain what and why vs. how
- write comment in text editor and then paste
