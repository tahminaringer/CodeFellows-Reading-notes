# Reading 09 Forms & JS Events

## HTML Chapter 7

### Forms
- `<form>` 
  - Element that has some built attributes for sending data across an http connection.
  -event for submitted data imput by the user
  - can speck to its children that are form type
- mailing lists, search box, forms, registering member, online shopping
  - `text input` used as email addresses and names
    - `<input>` used to creat several different form controls
    - type='text - it creates a single line input
  - `pasword input`
  - `text area` messages/coments
  - `radio buttons` multiselection buttons
  - `checkboxes` select boxes
  - `drop-down boxes` user picks on number of options from list
  - `submit button`
  - `image buttons`
  - `file upload` allows users to upload files

### Form Structure- `<form>`
- always carries the action attribute and will usually have a method and id attribute too
- `action attribute` every form requires an action attribute. its value is the URL for the page on the server that will receive the information in the form
- `<input>` type="password" 
- `<textarea>` used to creat a multi-line text imput
- **Radio Button** allow users to pick just one of a number of option
- Multiple select boxes `<select>`
- `<button.`- allows users more control over how thier buttons appear and to allow other elements to appear inside the button
- `<label>` accessible to vision impaired users

## HTML Chapter 14 Lists, Tables & Forms

- **Table properties**
  - width, padding, text-transform, letter-spacing, font-size, border-top/bottom text-align, background color, :hover
  - Use `empty-cells` property to specify if empty cells border should be shown or not.
  - **vursor styles** allows you to control the type of mouse cursor that should be displayed to users
  - **Web Dev Toolbar** provides tools to show you the CSS styles that apply to an element when you hover over it

## JS Chapter 6 Events

- **How events trigger JS Code**

 1. Select the element nodes you want the script to respond to
 2. Indicate which event on the selected node will trigger the response
 3. state the code you want to run when event occurs
 
- Three Ways to Bind an Event to An Element
  
  1. HTML Event Handlers
  2. Traditional DOM Event Handlers
  3. Dom Level 2 Event Listeners

- Creating event listeners for a lot of elements can slow down a page but event flow allows you to listen for an event on a parent element.
- Event object has methods that change: the defalt behavior of an element and how the elements ancestors respond to the event
- *User Interface Events* Occur as a result of interactio with the browser windo rather than the HTML page contained within it
- *Load* used to trigger scripts that access the contents of the page
- *Focus & Blur Events* HTML elements you can interact with such as links and form elements can gain focus
- *Mouse* are fired when the mous is moved and also when its buttons are clicked
- *Keyboard Events* are fired when a user interacts with the keyboard
- *Form Events* are commonly used with forms
- *Mutation Events & Observers* Whenever elements are added to or removed from the DOM its structure changes. which triggers a mutation event
