# Codecademy
Code from some Codecademy courses

CSS colors:

HEX 	    RGB

\#2e69a3 	rgb(46,105,163)

\#d8dabe 	rgb(216,218,190)

\#dabece 	rgb(218,190,206)

\#799575 	rgb(121,149,117)

In the CSS above, font-size is set to 60px. In CSS, size can be assigned in pixels (px), rems, or ems.

- pixel (px): Standard unit of measurement for sizing fonts and other HTML elements.

- rem: Represents the default font size for the web browser. Rems can be used to ensure that HTML elements scale in proportion to each other on various web browsers and screen sizes. On most web browsers, 1rem is equivalent to 16px, 2rem is equivalent to 32px (a doubling), 3rem is equivalent to 48px (a tripling) and so on.

- em: A relative value that changes in proportion to the size of the parent element. For example, if a parent element has font-size: 20px;, child elements with font-size: 1em; would be equivalent to 20px. Child elements with font-size: 0.5em; would be equivalent to 10px (a halving) and so on.

We will primarily explore px and rem values since these are the most commonly used today. 


Web Concepts

- CSS: Language used to style websites. Colors, fonts, and page layouts for a site are managed using CSS.

- CSS Selectors: specifies exactly which HTML elements to style

  - class selectors: used to target classes of HTML elements

  - id selectors: used to style an HTML element which has an id attribute.

- External Stylesheet: CSS file that styles an HTML file externally via the HTML link element.

CSS Properties

- font-family: sets font for a CSS selector.
- color: sets font color for the CSS selector.
- font-size: sets font size for text.
- background-image: sets a background image of your choosing for a given selector.


Observe the CSS box model diagram to the right:

- content: Includes text, images, or other media contained within an HTML element.

- padding: The space between the content and the border. You can think of this like inner space.

- border: The outline of an HTML page element. You can think of it like a picture frame that contains the element.

- margin: The space between the HTML page element and the next nearest element(s).


Using borders, padding, and margins allows us to control boundaries and space for individual HTML elements.

But what CSS properties are available to move elements around on the page and create unique page layouts? The CSS display and position properties help accomplish this.
Display

Not all HTML elements are displayed on a page in the same way. Display types determine how HTML elements will be arranged in relation to each other.

The diagram to the right illustrates the block and inline display types.

In the diagram, notice:

- The two dotted rectangles represent webpages.

- HTML heading, paragraph, and unordered list elements are block level: each appears on its own line on the webpage.

- HTML image and anchor elements are displayed inline: they appear on the same line as their neighboring elements on the webpage.


In the web browser, the gallery images that were arranged neatly in rows are now stacked on the left side of the webpage.

The CSS display value that arranged the images, flex, has been removed. In addition to other capabilities, flex can be used to easily align multiple page elements horizontally.

In the example code below, there is a div with class parent:

<div class="parent">
   ...
</div>

To make children of the div align horizontally on the webpage, in CSS we can use:

.parent {
  display: flex;
}

Children elements of the div with class parent will now align horizontally. We can make sure no child element moves off the page by using flex-wrap: wrap;:

.parent {
  display: flex;
  flex-wrap: wrap;
}

Finally, to center rows of children elements, we can use justify-content: center;:

.parent {
  display: flex; 
  flex-wrap: wrap; 
  justify-content: center;
}

Web Concepts

- CSS Box Model: illustrates the space and boundary properties of an HTML element that can be controlled using CSS.

CSS Skills

- border: sets the outline of an HTML page element, like a picture frame that contains the element.

- padding: sets the amount of space between an element's content and its border.

- margin: sets the amount of space between an HTML element and the next nearest element(s).

- display: property that determines how the selected element will be arranged in relation to other HTML elements on the page.

- inline: display value used to arrange HTML elements on the same line as neighboring elements.

- flex: display value that allows us to easily align multiple page elements vertically or horizontally.

- float: property used to float HTML elements left or right of neighboring elements.

- position: property used to position HTML elements in exact locations on a webpage.

