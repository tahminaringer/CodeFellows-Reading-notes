# Reading Assignment 01 - HTML & JavaScript

## HTML Chapter 1

- HTML is the structure of the page
- **Atribute** provide additional information about the contents of an elelment.
- Atributes are made up of two parts, **name** and **value**
- `<Head>` contains the info about the page, usually includes a `<title>`- which shows on tab or top of browser.
- `<body>` the main content of the page

## HTML Chapter 8

- Every web page must start with a `<DOCTYPE>` which is a declartion to tell the browser which version of HTML is being used
- `<!--comment-->` is used to make comments within HTML
- **ID Attribute** used to uniquely identify element from other elements.
  -Its value must start with a letter or underscore, never a number or other character.
  - no two elements on same page can can have the same value for their ID.
  - helps to style in CSS
  - ID attributes can allow script to work with that paticular element
  - Is know as a **Global Atribute** since it can work on any element.
- **Class Attribute** Used to identify multiple elements from being different from the other elements.
- **Block Level Elements** Always appear to start on a new line. Examples- `<h1> <p> <ul> <li>`
- **Inline Elements** Will appear to continue on the same line. examples- `<a> <b> <em> <img>`
- `div` allows you to group a set of elements together in one block-level box. example to contain all the elements for your header.
  - Using an ID or Class attribute with `<div>` allows you to create CSS rules to indicate how much space the element should take up
  - Makes it easier to follow code. note add a comment after closing `</div>` shows which opening tag it corresponds to.
- **Grouping Text & Elements Inline** `<span>` is used to contain a section of text or contain a number of inline elelments.
  - Makes easy to style with CSS
- **IFRAMES** `<inframe>`
  - used to embed images onto a page, such as google maps. Uses the following attributes
  - `src` specifies the URL of the page to show in the frame
  - `height` specifies the height of the iframe in pixels
  - `width` specifies the width of the iframe in pixels.
  - `scrolling` indicates whether the ifram should have scrolbars or not. Not supported in HTML5
  - `frameborder`Indicates whether the frame should hav ea border or not. Not supported in HTML5
  - `seamless` New HTML5 attribute can be applied where scrolbars are not needed.
-`<meta>` lives inside the `<head>` element and contains information about the web page
  - Not visible to users, tells search engines about your page, who created it and wheather it is time sensitive
  - empty element does not contain a closing tag
  
## HTML Chapter 17

- **Header & Footer** can be used the main header or footer or for an individual article or section within a page
- **Navigation** contains the major navigational blocks of the site.
- **Articles** acts as a container for any section of a page that can stand alone
- **Aside** has two purposes. 
  -when inside an article contains information related to the article but not essential to it overall meaning. ex: pullquotes or glossary.
  - when used outside of the `<article>` acts as a container for content that is related to the entire page.
- **Sections** groups related content together
- **Heading** `<hgroup>` group together a set of one or more `<h1>` through `<h6>` elements
- **Figures** `<figure>` `<figcaption>` used when the content references the element
- **Linking Around Block-Level Elements** `<a>` allows you to tun an entire block into a link
- **Helping older Browsers Understand** Inclued a line of CSS stating which new elelments should be rendered as block-level elements.

## HTML Chapter 18

- Design for the target audience
  - **Individuals**age, who will it apeal to, what country do your visitors live in, urban or rual, average income, level of education, marital family status, occupations, hours they work, how often use the web, what kind of device do they use to search the web.
  -**Companies** Size of company, whats the position of people in company that visit site, will they be using the site for themselves or someone else, what is their budget.
- Why do people visit your site
  - **Key motivators** for entertainment, achieve specific goal, is goal personal or professional, is it essential or luxury
  - **Specific Goals** searching form general information or something specific, are they familiar with service or product, do they need an introduction to product, do they need info in order to purchase, do they need to contact you
- Define what information your visitor needs
- Take into account how often people will visit site, does it need to updated more frequently
- Create a **Site Map** This breaks down each section of the website into individual pages and their content
- **Wire Frame** sketch of key information that needs to go on each page of the site.

### Designing a Web Page

- **Visual Hierarchy**- order in which your eyes perceive what they see
  - Use **size** to grab users attention, 
  - **color** forground and background color can draw attention,
  - **Style** element may be the same size but have different style applied to help it stand out.
- **Grouping and Similarity**
  - *proximity* items placed close together
  - *closure* create single or recognisable pattern or form
  - *Continuance* When place in a line or curve elements are seen to be more related
  - *White Space* placing related items closer together and leaving a bigger gap between unrelated items
  - *color* background color placed behind emphasizes their connection
  - *borders* line drawn around the border of the group or between it and it's neighbors
  - *consistency* having consistent style throughout
  - *Headings* tells user if content is relevent to them
- **Designing Navigation**
  - Concise, quick and easy to read
  - Clear- predict information they will find on pages
  - Selective- only reflect the navigation of the sight other items such as login should be placed elsewhere
  - Context- Tells user where they are in the website. This is done by using color or visual marker
  - Interactive- link should be proper size and link should change when user hovers overtop
  - Consistent- Larger site more nav items. Keep primary navigation the same.

## JS Chapter 1

- **Script** a series of instructions for a computer to follow step by step
- To write a script define the goal then list the tasks
  1. define the task you want to achieve
  2. Design the script by dividing the goals out into a series of tasks.
  3. Code each step
- Work out individual tasks using a **Flowchart**
- Breakdown each individual task into a sequences of steps.
- **Objects** things, physical object
  - Each object can have it's own property, events or methods
-**Properties** Characteristics- what defines the object or characteristics of object
- **Names/values** tells you about instance of object
- **Event** Computer's way of saying "hey this just happened"
  - Scripts use different events to trigger different types of functionality.
- **Method** represents how people or things interact with an object.
-**Window Object** the browser represents each window or tab using a window object. Location property of window object will tell you URL
- **Document Object** represents an HTML page
  - can access and change content users see and interact with it.
  - *Properties* describe characteristics of the current web page
  - *Methods* perform tasks associated with the loaded document in browser
  - *Events* you can respond to events, user clicking an element

## How to Write sript for a webpage

- *HTML* Content layer- gives page structure and semantics.
- *CSS* Presentation layer- Enhances HTML
- *JS* Behavior Layer- Change how page behaves and add interactive features.

## How to Use Objects and Methods

`Document.write('Good Afternoon!');`

- **Object** The `Document` object above represents the entire webpage.
  - The object has several methods and properties known as memebers of that object.
  - can access the members of an object by using a dot `.` between the object name and it's member you want to access.
- **Method** The `write()` method above allows new content to be written into the page where the `<script>` element sits in HTML
- **Parameters** the information inorder for the task to work. This data is given inside parentheses of the method

