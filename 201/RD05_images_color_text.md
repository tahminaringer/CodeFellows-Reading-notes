# Read 05 Images, Color, Text

## HTML Chapert 5 - Images

- helps engage users in site
  - relevent
  - convey information
  - convey the right mood
  - be instantly recognisable 
  - fit the color palette
- **Stock images** Images you pay to use
- Store images in a folder called images
- `<img>`is used to link images to a page
  - *src* tells browser where image can be found
  - *alt* provides a text description
  - *title* provides additional information about the image
- **height/width** specifies height and width in pixels
`<img src=" alt=" width=" height=" align="left">`
- Place image tage before a paragraph, inside the start of a paragraph, in the middle of a paragraph
- **align** you can align `left` `right` `top` `bottom` and `middle` using the `align=""`
- **image format** Save images in jpeg, gif, or png format
  - wrong format may affect image quality
  - images with many colors use jpeg
  - use gif or png wen saving images with few colors or large ares of the same color
- **Dimensions** save images at the same width and height you want them to appear on the page
- **cropping** careful of loosing valuable info
- always set image size in px
- when creating images for print save them at 300 dots per inch (DPI) or higher to make sure they look good
- **Vector images** logos are created in vector format- created by placing points on a grid and drawing lines between those points
  - color can be added to fill in the lines
- **Animated GIFS**
  - remember each extra frame of the image increases file size and loading time
  - Only suitable for simple illistrations
**Transparency** image that is partially transparent


## HTML Chapter 11 Color

- **RGB Values** express colors in how much red, green and blue are used to make color
- **Hex Codes** six digit codes that represent the amount of red, green and blue preceded by a #
- **Color Names** 147 predefined color names
- **Background Color** Treats each HTML element as if it appears in a box. Property sets background for box
- **Contrast** when picking colors make sure they have contrast
  - Low contrast- text is harder to read
  - high contrast- text easier to read
  - Medium contrast- for long spans of text, reducing the contrast a little improves readability
_ **Opacity** 
- **HSL Colors** Hue saturation and lightness values
- **HSLA** Hue saturation, lightness and ALPHA- transparency

## HTML Chapter 12 TEXT

- **Typeface Terminology**
  - *serif* extra details on the ends of main strokes
  - *san-serif* strait ends
  - *monospace* every letter in mono space is the same width
  - *weight* light, medium, bold, black
  - *style* normal italic oblique
  - *stretch* condensed regular extended
- **Choosing typeface** for font to show up it must be installed on browser of users computer
- **font-family** allows you to specify the typeface
- **font-size** Allows you to adjust font size
- **font-face** use a font, even if it is not installed on the computer. specifies path to a copy of the font which will be downloaded if not on users computer
**text-transform** allows you to transform the text by giving one of following values
  - uppercase
  - lowercase
  - capitalize - causes the first letter of each word to appear capitalized
- **text-decoration** allows you to specify the following values
  - none- rmoves any decoration already aplied
  - underline
  - overline- this adds a line over the top of the text
  - line-through- adds a line through words
  - blink animates the text to make it flash on and off
- **line height** vertical space between lines of text
- **letter-spacing/word-spacing** space between each letter or word
- **text-align** 
  -left
  -right
  -center
  -justify- every line except for last should be set to take up full width of the containing box
- **vertical** used with inline elements such as `<img>` 
- **Text-indent** allows you to indent the first line of text within element
- **text-shadow** creates a drop shadow
- **first-letter, first-line** can specify different values for the first letter or first line of text inside element
- **:link** allows you to set styles for links that have not yet been visited
- **:visited** sets styles for links that have been clicked on
- **:hover** Changes the appearance of a thing like a button when a user hovers over it
- **:active** applied when an element is being activated by a user. made to feel like pushing a button
- **:focus** Any element you can interact with.
- **Attribute Selectors**
  - existence- matches a spcific attribute `[]`
  - Eaquality- matches a specific attribute with a specific value`[=]`
  - space - mathces a spcifdic attribute whose value appears in a space separated list of words `[~=]`
  - Prefix- Mathches a specific attribute whose value begins with specific string `[^=]`
  - Substring- `[*=]`
  - suffix `[$=]`
  