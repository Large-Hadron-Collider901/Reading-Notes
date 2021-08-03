# HTML Forms

## Form Structure
* `<form>` - this is where form controls such as the action, method, and ID attributes live
* `action` - the value of the action attribute is going to be the URL for the page on the server that will recieve any info that's submitted in the form
* `method` - there are two methods we can use to send forms
 - `get` is ideal for short forms such as search boxes or for any information we are retrieving from the user that does *not* need to be added to or deleted from a database
 - `post` - some situations that call for using the `post` method include if our form:.....allows users to upload a file, is very long, contains sensitive data, adds info to and deletes info from a database

 **Example:** 
 ```
 <form action="http://www.whereverYoureSendingTheInfo.com" method="get">
 <p>this is where the form controls go
    </p>
 </form>
 ```

 ## Form Controls 
 * We can use the `<input>` element to create form control attributes such as:
   - **type:** the value of this attribute determines what kind of input they will be creating (for example: `type="text"` creates a single line of text input)
   - **name:** each form control requires a name attribute in order to tell the server which form control each piece of data was entered into. (for example: username and password) 
   - **maxlength:** limits the number of characters a user can enter in the text field

## Input types
* Text input
* Password input
* Radio button
* Checkbox
* Drop down list box
* Multiple select box
* File
* Submit button
* Image button

## HTML5: Form Validation
Form validation has traditionally been performed using JavaScript, however HTML5
introduces validation and leaving the work to the server! Here are some benefits of
form validation:

- Ensures the user enters info in a form that the server can understand when the form is submitted
- Reduces the amount of work the server has to do
- Helps users catch any errors in the input they have provided

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

# JavaScript Events

## Event Handling
There are three steps involved in triggering JavaScript code, these steps are called *event handling*

### Select Element
1. Select the element node(s) we want the script to respond to
  * If we want to trigger a function when a user clicks on a link, then we need to get the DOM node for that link element using DOM query

### Specify Event
2. Indicate which event on the selected node(s) will trigger the response 
  * Some examples of events we can choose from include: onmouseover, onclick, onchange, onload, onkeydown
### Call Code
3. Enter the code you want to run when the event occurs
* When the event occurs on a specified element it will trigger a function

## Types of Event Handlers
Event handlers let us indicate which event we are waiting for on any particular element. There are 3 methods we can use to bind an event to an element

1. HTML Event Handlers (bad practice, old method)
2. Traditional DOM Event Handlers 
3. DOM Level 2 Event Listeners

## Types of Events
* W3C DOM Events
* HTML5 Events
* BOM Events
* User Interface Events 
* Load
* Focus & Blur Events
* Mouse Events
* Click
* Keyboard Events
* Form Events
* Mutation Events
* HTML5 Events
