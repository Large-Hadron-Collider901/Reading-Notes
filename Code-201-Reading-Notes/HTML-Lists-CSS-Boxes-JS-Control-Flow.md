# HTML Lists

There are three types of lists in HTML:

 1. **Ordered List:** Organized by number, a good choice for lists that consist of a certain number of steps that need to be done in order, or for lists that require a format with sections

```
Ordered lists open with an <ol> element and close with an </ol> element
Each list item opens with a <li> element and closes with a </li> element
HTML Example:                     Result:
<ol>
   <li>List item</li>             1. List item
   <li>List item</li>             2. List item
   <li>List item</li>             3. List item
</ol>
```

2. **Unordered List:** Organized with bullet points

```
Unordered lists open with a <ul> element and close
with a </ul> element.
The list items in an unordered list have the same
syntax as the list items in an ordered list

HTML Example:                      Result:
<ul>
  <li></li>                        • List item
  <li></li>                        • List item
  <li></li>                        • List item
</ul>
```


3. **Definition List:** A vocabulary list that is made up of a set of terms along with their definitions. The structure of a definition list is a *little bit* different from the other types of lists.

```
 A definition list opens with a <dl> element and closes with a </dl> element. The term that is going to be defined (definition term) will go between an opening <dt> element and a closing </dt> element. Then, the definition for that term will be contained with an opening <dd> element and a closing </dd> element

HTML Example:                     Result:

<dl>
  <dt></dt>                       Term
  <dd></dd>                          Definition
  <dt></dt>                       Term
  <dd></dd>                          Definition
  <dt></dt>                       Term
  <dd></dd>                          Definition
</dl>
```

**Nested Lists**

```
You can also put a second list inside an <li> element to make a nested list

HTML Example:                      Result:

<ul>
   <li>Item</li>                   • Item
   <li>Item                        • Item
     <ul>                             • Nested item
       <li>Nested item</li>           • Nested item
       <li>Nested item</li>           • Nested item
       <li>Nested item</li>        • Item
    </ul>
   </li>
  <li>Item</li>
</ul>
```

# CSS Boxes

In CSS, each HTML element has it's own box. The dimensions of a box can be adjusted using their width and height properties, but there are several other adjustable elements that make up a box such as borders, margins, and padding. You can use CSS to customize the different properties in a box, allowing you to organize and style your content as well as increase usability across devices with different sized screens!

Each box has three properties that can be adjusted for appearance:

1. **Border:** The edge that separates one box from another
2. **Margin:** The space that sits out side the edge of the border
3. **Padding:** The space between the border and the box along with any content contained within it

<br />

Here are some examples of organizational  
box properties:

* min-width 
* max-width 
* min-height  
* max-height
* overflow

These properties improve the legibility of a web page but ensuring that the content does not appear smaller or larger than the specified values, allowing the content to look neat and organized no matter what size screen it is being viewed on.
<br />

Here are some examples of stylizing box
properties:

* margin
* padding
* border 
* border-width
* border-style
* border-color
* text-align
* display
* visibility
* border-image
* box-shadow
* border radius
<br />

Definitions in this content were taken from the textbook
*HTML And CSS Design And Build Websites* By John Duckett
and can be found in Chapter 3: “Lists” (pp.62-73) and 
Chapter 13 "Boxes" (pp. 300-326)

<br />

# JavaScript Control Flow

### Data Types
Data types refer to the different kinds 
of data that we will be storing in variables.
Here are the main data types we will be working
with in JavScript:

* **Numeric** - This data type handles numbers. 
Numeric data types can be used for tasks such
as determining the size of a screen, moving the
position of an element on a page, or setting the
amount of time an element should take to fade in.

* **String** - The string data type consists of 
letters and other characters. Strings can be used
when working with text. They are frequently used
to add new content into a page and they can contain
HTML markup.

* **Boolean** - Boolean data types can have one of
two values: true or false. Booleans are helpful
when determining which part of a script should run.

### Arrays
An array is a special type of variable that 
stores a list of values rather than just one. 
They should be used whenever you are working
with a list or set of values that are related
to each other.



### Switch Statements
A switch statement starts with a variable called the switch value. 
Each case indicates a possible value for this variable and the 
code that should run if the variable matches the value. 

### Loops
The purpose of a loop is to check a condition. If it returns
true, a code block will run. Then the condition will run
again and if it still returns true, the code block will 
run again. It repeats until the condition returns false.
There are three common types of loops:

1. **For:** For loops (the most common type of loop) are 
used to run code a specific number of times. In a for loop, 
the condition is usually a counter which is used to tell 
how many times the loop should run.

2. **While:** If you do not know how many times the code
should run, you can use a while loop. Here, the condition
can be something other than a counter, and the code will
continue to loop for as long as the condition is true.

3. **Do While:** This loop is very similar to the while
loop, but has one key difference - it will always run
the statements inside the curly braces at least once,
even if the condition returns false.  


Definitions in this content were taken from the textbook
*JAVASCRIPT & JQUERY Interactive Front-End Web Development*
By John Duckett and can be found in Chapter 2: “Basic JavaScript
Instructions” (pp.62-73) and Chapter 4: “Decisions and Loops”
(pp.162-182) 


