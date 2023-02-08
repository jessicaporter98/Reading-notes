# CSS 

**CSS** otherwise known as *cascading styling sheets*


*CSS* is a language for specifying how documents are presented to users — how they are styled, laid out, etc.

 Using **CSS** , you can control exactly how HTML elements look in the browser, presenting your markup using whatever design you like.

**CSS** can be used for very basic document text styling — for example, for changing the color and size of headings and links. 

It can be used to create a layout — for example, turning a single column of text into a layout with a main content area and a sidebar for related information.
 It can even be used for effects such as animation.

 this is for red text:
 h1 {
  color: red;
  font-size: 5em;
}

In this above example, the *CSS* rule opens with a selector.
 This selects the HTML element that we are going to style. In this case, we are styling level one headings (<h1>).

We then have a set of curly braces { }.

Inside the braces will be one or more declarations, which take the form of property and value pairs.
 We specify the property (color in the above example) before the colon, and we specify the value of the property after the colon (red in this example).

This example contains two declarations, one for color and the other for font-size. Each pair specifies a property of the element(s) we are selecting (<h1> in this case), then a value that we'd like to give the property.

CSS properties have different allowable values, depending on which property is being specified.
 In our example, we have the color property, which can take various color values. 
 \We also have the font-size property. 
 This property can take various size units as a value.

As there are so many things that you could style using CSS, the language is broken down into modules. 

The browser support status is shown on every MDN CSS property page in a table named *"Browser compatibility"* . Consult the information in that table to check if the property can be used on your website. 

An external stylesheet contains CSS in a separate file with a .css extension.

h1 {
  color: blue;
  background-color: yellow;
  border: 1px solid black;
}

p {
  color: red;
}


The href attribute of the <link> element needs to reference a file on your file system.

 In the example above, the CSS file is in the same folder as the HTML document, but you could place it somewhere else and adjust the path. Here are three examples:

<!-- Inside a subdirectory called styles inside the current directory -->
<link rel="stylesheet" href="styles/style.css" />

<!-- Inside a subdirectory called general, which is in a subdirectory called styles, inside the current directory -->
<link rel="stylesheet" href="styles/general/style.css" />

<!-- Go up one directory level, then inside a subdirectory called styles -->
<link rel="stylesheet" href="../styles/style.css" />

