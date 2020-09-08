# Read: 06 - JS Object Literals; The DOM

## How to understand the problem domain

- **make problem domain easier** cut out cases and narrowing your focus to a paticular part of the problem
  - understand the parts of the problem domain before expanding the problem domain
- **Understand problem domains** spend the time to talk over the problems with your client instead of assuming you know how to proceed

## JS Chapter 3 Object Literals

- **Objects** group together a set of variables and functions to create a model of something you would recognize in real life
  - similar to an array
  - object is the curly braces and thier contents
  - you can access the properties/methods of an object by using a dot notation or square brackets
    - **pros**
      - describe our data more
      - no longer need to perform a loop to validate and lookup information
    - Object Ex:

    ```
    Jacob {
        name: 'Jacob',
        age: 30,
        title: 'instructor'
      }

      ```

    - Array Ex:

    `Jacob = [name, 30, title]`

    - `this` is a key word in JS, that references the current object that our block of cade points to.

  - **properties** variables within an object
    - value can be a strig, mumber, boolean, array or an object
  - **methods** functions within an object
    - value of method is always a function
  - **key** name and value of properties and methods
    - Object cannot have two keys with the same name.
  - **accessing data from an object**
  ```bracket notation

  Jacob['name]

## JS Chapter 5 Document Object Model

- lives in the global runtime environment.
- we can call out to this object, within any code block that runs in the browser
- The JS was conceived as a multi runtime language.
  - The runtime was responsible for providing the functionality
- A built in API(application program interface)

- **DOM tree** model of a web page created by the browser, stored on the memory consisting of four main nodes.
- **Document Node** represents the entire page
- **HTML elements** describe the structure of the HTML page
- **Attribute Nodes** HTML can carry attributes and these are represented by attribute nodes in the DOM tree
- **Text nodes** once you have accessed an element node you can then reach the tect within that element.
- Two Steps of accessing and updating the DOM Tree
  1. locate the node that represents the element you want to work with.
  2. Use its text content, child elements, and attributes
- **DOM Queries** Methods that find elements in the DOM tree
- **Accessing Elements**
  - `getElementById('id')` selects an individual element given the value of its id attribute
    - returns a single element
  - `querySelector('css selector')` Uses CSS selector syntax that would select one or more elements.
    - returns a single element
    - `querySelectorAll()` returns a NodeList of all of the matches.
  - `gueElementsByClassName('class')` selects on or more elements given the value of their class attribute
  - `querySelectorAll('css selector')` Uses CSS selector syntax to select on or more elements and returns all of those that match.
  - `getElementsByClassName()` method allows you to select elemetns whose class attribute contains a specific value.
  - `getElementsByTagName()` method allows you to select elements using their tag name

- **nodelists** a collection of elemetn nodes. each node is given an index number. Looke like arrays and are number the same.
- **item() Method**returns an individual node from the NodeList.
- **Array Syntax** you can access individual nodes using `[]` similar to that used for arrays
- **Trabersing the DOM**
  -parentNode-
  -PreviousSibling/nextSibling
  -firstChild/lastChild
- **textContent** to collect the text from the element and ignore any markup inside the element
- **innerText** AVOID if possible
- **InnerHTML**
  - Approach- can be used on any element node. used to retrieve and replace content.
  - Adding content -
    1. store new content as a string in a variable
    2. select the element whose content you want to replace
    3. set the elements innerHTML property to be the new string.
  - removing content - to remove all content from an element you set innerHTML to an empty string
- **DOM manipulation methods**
  - approach - DOM manipulation refers to a set of DOM methods that allow you to create element and text nodes and then attach/remove them to the DOM tree.
  - adding content- To add content, you use a DOM method to create new content one node at a time and store it in a variable.
  - Removing content- you can remove an element from the DOM tree using a single method.
- **Adding Elements using DOM manipulation**
  - `createElement()` - you start by creating a new element node
  - `createTextNode()` - create a new text node
  - `appendChild()` - adds it to the DOM tree
- **Removing elements via DOM manipulation**
  1. Store the element to be removed in a variable
  2. Store the parent of that element in a variable
  3. Remove the element from its containing element
    - `removeChild()`
- `document.write()` adds content that was not in the original source code to the page,(use rarely advised)
- `element.innerHTML` lets you get/update the entire content of any element as a string
- **Cross-site Scripting (XSS) Attacks** an attacker could gain access to your user's accounts.
  - **validate input going to the server** 
    1. *validation* only let visitors input the kind of characters they need to when supplying information
    2. double check validation on the server before displaying user content/storing it in a database
    3. database may safely contain markup and script from trusted sources.
    4. as your data leaves the database, all potentially dangerous characters should be escaped 
    5. Make sure that you are inserting content generated by users into certain parts of the template files.
    6. do not create DOM fragments containing HTML from utrusted sources