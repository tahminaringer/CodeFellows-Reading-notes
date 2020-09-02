# Structue Web Pages With HTML

## **Chaper 18**

## Who is the site for

- Who is the target audience - demographic, age, size of company, etc
- Why target audience visits site
- Modivation to visit site
- Goal so visitor visiting site
- Do they need to be educated on site or are they informed
- time sensitive information
- will they need to contact you

## What  are visitors trying to achieve

- find key tasks and motivations
- create list of reasons why visiting site

## What info your visitor needs

- do they know your product
- What is special about your product
- What are the features of your product
- create relevence to customer base

## How often customer visits site

- trending websites need frequent updates
- service based websites need less updating

## Site Map

- diagram of pages
- card sorting
- site map- beguins with homepage

## Wire Frames

- simple sketch of key information
- DO NOT include colorscheme font choices etc

## Visual Heirachy- order which your eyes percieve what they see

- Size- style so larger elements are what grab users
- Color- adding color draws attention
- Style- styling can help elements stand out
- Images- draw attention and attract the eye and create contrast

## Grouping Similarity

- Proximity- items are placed close together/percieved as related
- Closure- coplicated arrangement look for recognizable form/pattern
- Continuance- placed in line or curve considered more related
- White Space- placing related items together and giving more space between unrelatable items
- Color- background color placed behind items ephasizes relatable items
- Borders- line drawn around grouping shows relatability
- Consistency- using some fonts and styling thoughout
- Headings- tells users if relevent to them

## Designing Navigation

- Consise- quick and easy to read
- Clear- users can predict information they will see on pages
- Selective- reflects sections/content of site
- Content- provides content and location on website
- Interactive- appropriate size, change color and visually distict
- Consistent- keep primary navigation the same

## **Chapter 1**

## HTML

- Discribes the stucture of the web page
- Text documents
- Most elements have opening and closing tags
- Attributes tell us more about elements `<p lang="en-us">Paragraph in English</p>`
- Atributes require a name and value

## **Chapter 17**

- Set of elements to divide up page

  - `<div id="page">, <header>,`
  - `<div id="content">, <article>`
  - `<aside>`
  - `<footer>`

- Header/Footer- cand be used for top or bottom of page or for individual article or section

  - each article and section can have their own header and footer

- Navigation- contains primary navigational blocks
- Articles- acts as container of a section of a page

  - article elements can be nestled inside eachother

- Asides-
  
  - Used inside an article element contain information that is related but not essential, pull quote, glossary
  - Used outside article acts as content realated to entire page

- Sections- groups related items together also have own heading
- Heading groups- `<hgroup>` groups together a set of one or more h1-h6
- Figures- `<figure> <figcaption>` contain any content that is referenced form the main flow of article
  
  -only use when the content references the element and helps the flow of the page
  - usage- images, videos, graphs, diagrams, code samples, text that supports the main body of an article
  - Should also include a `<figcaption>` which provides text discription
  
- Sectioning Elements
  - `<div>` important way to group together elements

- Linking Around Block-Level Elements
  - allows you to turn an entire block into a link `<a>` by wrapping elements in the above element.

- Helping Older Browsers Understand

  - include line of CSS to show which elelment should be rendered as block-level elements

    - `header. section. footer. aside. nav. article. figue. figcaption {display: block:}`

## **Chaper 8**

## The Evolution of HTML

- HTML 4- similar to HTML 5 with elements eliminated
- XHTML 1.0 works seemlessly with other programs in XML
- HTML5- do not have to close all tags/new elements and attributes will be introduced

- **DOCTYPES**
  
  - Each web page should begin with a DOCTYPE declaration to tell browser which version of HTML is being used
  - Helps render page correctly

- **Comments in HTML** to add code that will not be visible
  
  - `<!--comment goes here-->`

- **ID Attribute**identify that element from other elements
  - value should start with leter or underscore never number
  - helps style in CSS
  - JS allow the script to work with that particular element

- **Class Attribute** way to identify several elements
  
  - helps differentiate importance
  - helps differentiate links that point to outside your site or within
  - value can be used on headings and links too
  - do not affect presentation unless CSS rule is inplace
  
- **Inline Elements** -appear to continue on same line as neighbouring elelments

-**Grouping Text & Elements in a Block**

- `<div>` tag allows you to group a set of elements/ ex: contain all elements in header
  - Using an ID or Class attribute on the dive element means you can incorperate CSS style rules
  - easier to follow code
  - helpful to add comment after closing

- **Grouping Text & Elements Inline**

- `<span> inline equivelent of <div>`
- control the style of the content by using CSS

- **iframes** `<iframe>`
- little window into page such as embeded map on page

  - **src** the src specifies URL of the page to show in the fram
  - **height** The height attribute specifies the height of the frame in pixels
  - **width** specifies the width of the iframe in pixels
  - **scrolling** not supported in HTML5, indicates wheather iframe should have scroll bars or not
  - **frameborder** Not be supported in HTML5, indicates whether the frame should have a border or not
  - **seamless** can be applied to an iframe where scrollbars are not desired. Does not need value

- Information about your pages
  
  - `<meta>` lives inside the head element contains info about that web page

    - tells search engines about page
    - does not have closing tag
    - commonly used name attributes- descrption, keywords, robots, author, pragma, expires

- **Escape Characters** show symbols such as copy write trademark, currancy, mathematical characters and punctuation marks.
  - See page 194 for list
