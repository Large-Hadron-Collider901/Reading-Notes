## What is CSS?##

CSS is a language which is responsible for the style, layout, and other presentation features of a document
Here are some examples of how CSS can be used:
* Change color and size of headings or links
* Create a layout- (adding a main content area, sidebars, columns, etc)
* Animation

CSS is a rule-based language
-define rules specifying styles yoiu want to apply to elements or groups of elements

The rule opens with a selector that selects the HTML element it is going to style

EX: <h1> in this case we are styling level one headings 

Next we have declarations which are property and value pairs inside curly brackets {}
 EX: {

    property ---> color: red 
     Font-size: 5em <--- value

 }

 **inidvidual property pages on MDN for quick reference**

 Three ways to insert CSS

 * Internal
 * External
 * Inline

 ### Internal CSS Examples

 <style
    h1 {   
        color: yellow;
        text-align: right;
  }>
  </style>

  ### External CSS ##
  It requires a link to some style.css file

  <link rel="stylesheet" href="style.css">

  ### Inline CSS ###

  In the html line dirrectly

  <p style="color: red; text-align:center">