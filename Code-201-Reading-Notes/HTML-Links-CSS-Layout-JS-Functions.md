# HTML Links
Types of links you will commonly see
on web pages:
* Links from one website to another
* Links from one page to another on
the same website
* Links from one part of a web page 
to another part of the same page
* Links that open in a new browser
window
* Links that start up your email 
program and address a new email to
someone

#### Writing Links

Here is an example of the syntax we
will need to use to create a link:

```
<a href="http://www.whatever-webpage-you-want-to-go-to.com">The text the user clicks on</a>
```
#### Linking To Other Sites
The value of the href attribute is the page that you want 
people to go to when they click the link. When you are 
linking to a different website, the value of href will be
the full web address for the site (known as an absolute URL

**Absolute URL:** This is the web address that you would 
type into a browser if you wanted to visit that specific
page. An absolute URL starts with the domain name for that
site and can be followed by the path to a specific page.

#### Linking To Other Pages On The Same Site
When you are linking to pages within the same site,
you do not need to specify the domain name in the
URL. Instead you can use a relative URL.

Here's an example of a link to a page on the same website
using a relative URL:

```
<a href="about-us.html">About-Us</a>
```

#### Email Links
To create a link that starts up the user's email program
and addresses an email to a specified email address, you
will still use the <a> element. However, the value of the
href attribute starts with mailto: followed by the email
address you want the email to be sent to. Here's an example
of how we would write this type of link

```
<a href="mailto:skye@example.com">Email Skye</a>
```
 #### Opening Links In A New Window
If you want to create a link that will open in
a new window, all you need to do is place the
target attribute in the opening tag following
the link. The value of this attribute should be
_blank. Below is an example of a link that
opens in a new window.

```
<a href="http://www.google.com" target="_blank">Google Search</a>
```
#### Linking To A Specific Part Of The Same Page
Before you can create a link that will bring
you to a specific part of the same page, you
will need to use the id attribute to identify
the points of the page your link will go to.

```
Lets say you want the link to take you to 
this spot in the page:

<h2>about me</h2>

You will need to add an id attribute
to your header 2. Like so,

<h2 id=about_me>about me</h2>

and then the link to take you
to about about me section will
look like this:

<a href="#about_me">About me</a>
```

#### Linking To A Specific Part Of Another Page
As long as the page you are linking to has
id attributes that identify specific parts
of the page, you can use a similar technique
to create a link that will take to you to
that section of a page. Just enter the link
to the page for the href attribute, followed 
by the # symbol, followed by the value of the 
id attribute that is used on the element you
are linking to. Here is an example of what 
linking to a specific part of another page will
look like:

```
<a href="http:/www.htmlandcssbook.com/#bottom">HTML AND CSS Book Bottom Section</a>
```


Definitions in this content were derived from 
Chapter 4: “Links” (pp.74-93) of the textbook 
*HTML & CSS Design And Build Websites* 
By Jon Duckett


# CSS Layout

## Key Concepts In Positioning Elements

#### Building Blocks
CSS treats each HTML element as if it is contained
in its own box. There are two types of boxes in
CSS:

1. **Block-Level Boxes:** Start on a new line and act as the main
building blocks of any layout. 

```
Examples of block-level elements:
 <h1> <p> <ul> <li>
 ```

2. **Inline Boxes:** Flow between the surrounding text

```
Examples of inline elements:
<img> <b> <i>
```

#### Containing Elements
 
Containing elements are block-level elements that 
contain another block-level element inside of it.
The outer box is the containing element or parent
element. 

#### Positioning Schemes

Positioning schemes in CSS allow you to control
the layout of a page. To specify the positioning
scheme, you will need to use the position property
or the float property. Here are some different 
types of positioning schemes used in CSS:

- **Normal Flow:** Every block-level element
appears on a new line, which positions each 
item lower down on the page than the previous one.

- **Relative Positioning:** This moves an element
from the position it would be in normal flow, 
shifting it to the top, right, bottom, or left
of where it would have been placed.

- **Absolute Positioning:** Positions the element
in relation to its containing element. Elements 
that are absolutely positioned move as users scroll
up and down the page.

- **Fixed Positioning:** A form of absolute positioning
that positions the element in relation to the browser 
window rather than to the containing element. Elements
with fixed positioning do not move when the users scroll
up or down the page.

- **Floating Elements:** Floating an element allows you
to take that element out of normal flow and position it 
to the far left or right of a containing box. The floated
element becomes a block-level element around which other
content can flow. 



#### Fixed Width Layouts

These layout designs do not change size according
to the size of the user's browser window. Measurements
tend to be given in pixels. 

#### Liquid Layouts

This type of layout design stretches and contracts 
depending on the size of the user's browser window.
Measurement tend to use percentages.


Definitions in this section were derived from 
Chapter 15: “Layout” (pp.358-404) of the 
textbook *HTML & CSS Design And Build Websites* 
By Jon Duckett

# JavaScript Functions

#### What Is A Function?

Functions allow you to group a series of statements together
in order to perform a specific task. They also provide a
way to store the steps needed to achieve a task.

#### Function Declaration
To declare a function, you will need to use the function keyword
followed by an identifier (the name you choose for your function)
followed by parentheses, followed by a set of curly braces containing
the statements that perform the task.

#### Calling A Function
After you declare the function, you can execute all of the statements
between the curly braces with just one line of code, this is referred 
to as "calling the function"

To run the code in the function, you use the function name followed by 
parenthesis  

#### Parameters
If a function needs information to work, you indicate what it needs to
know in the parenthesis after the function name. The items that appear
inside these parentheses are known as the parameters of a function. 
Inside the function, those words act like variable names.

#### Arguments
When you call a function that has parameters, you specify the values
it should use in the parenthesis that follow its name. The valuesc
are called arguments, and they can be provided as values or as 
variables. 

#### Variable Scope 
A variable's "scope" defines the area in which a variable can be
used

#### Local Variables
Local variables are variables that are created inside a function
and can only be used in that function. Local variables, have a 
local variable scope or function-level scope.

#### Global Variables
Global variables are created outside of a function and can be 
used anywhere in the script. These variables have a global scope.

Definitions in this section were derived from Chapter 3 (first part): 
“Functions, Methods, and Objects” (pp.86-99) of the textbook 
*JAVASCRIPT & JQUERY Interactive Front-End Web Development* By
Jon Duckett.