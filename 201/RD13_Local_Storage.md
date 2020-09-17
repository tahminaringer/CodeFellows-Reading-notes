# Local Storage

**Cookies downsides**-

- They slow down your web application by transmitting the same data over and over
- sending data unencryped over the internet
- cookies are limited to about 4 KB of data- enough to slow your app but not enough to be useful

**What is better**

- a lost of storage space
- on the client
- that persists beyond page refresh
- and isnt' transmitted to the server

- **userData** allows web pages to store up to 64KB of data per domain in a hierarchical XML-based structure
- **Local Shared Objects** it allows Flash objects to store up to 100 KB of data per domain
- **Gears** open source browser plugin aimed at providing additional capabilities in browsers. providing an API to an embedded SQL database

## HTML5 Storage 

- a way for web pages to store named ky/value pairs locally, within the client web browser.
- Web storage - Local Storage - DOM Storage
- check for HTML5 Storage-
`function supports_html5_storage() {`
`try {`
    `return 'localStorage' in window && window`
    `['localStorage'] !== null;`
`} catch (e) {`
    `return false;`
`}`
`}`
 Instead of writing this you can use `Modernizr`
 `if (Modernizr.localstorage) {`
 `}else {`
`}`
- storage is based on named key/value pairs.
- `setItem()` with a named key will silently overwrite the previous value
- `removeItem()` 
- data is stored as strings
- Web SQL Database- provides a thin wrapper around a SQL database.
- **Indexed Database API** object store
  - databases with records, each record has a sey number of fields.
