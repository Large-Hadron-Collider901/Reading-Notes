# HTML TABLES

* In html, we can add tables to a webpage by using the `<table>` element
* Each row in the table is indicated by the `<tr>` element
* A row contains various cells. Cells can be created using either the `<td>` element,
or if it is a header we will use the `<th>` element
* If we want to create cells of a table that span more than one row or column, we can
use the `rowspan` or `colspan` attributes
* For long tables, we can split the table into sections by using the `<thead>`, `<tbody>`
and `<tfoot>` elements 


Here's an example of how a table is structured in HTML:
```
<table>
  <thead>
    <tr>
     <th></th>
     <th scope="col">Column Header 1</th>
     <th scope="col">Column Header 2</th>
     </tr>
 </thead>
 <tbody>
  <tr>
    <th scope="row">Row Header 1</th>
    <td>data</td>
    <td>data</td>
 </tr>
 <tr>
    <th scope="row">Row Header 2</th>
    <td>data</td>
    <td>data</td>
 </tr>
 <!-- more rows like the two above here -->
 </tbody>
 <tfoot>
   <tr>
    <td></td>
    <td colspan="2">Data that spans for more than one section</td>
 </tr>
 </tfoot>
 </table>
```
---
# Domain Modeling
* A domain model is a communication tool designed to help stakeholders gain a better understanding of a problem domain
* The model describes various aspects of a specific problem using vocabulary that can be understood by both technical and business teams.
---

# JavaScript Constructor Functions

Suppose we are creating a database
of all the botanic gardens in the United States
that includes descriptive details about each garden. We could could go about this by manually creating each botanic garden object one by one

However, if we wanted to save a significant amount of time, we could streamline the process by using a constructor function.

* Constructor functions are templates for creating objects
* We can use it to create object instances that share similar properties
* The process of creating constructor functions is very similar to the way regular functions are created, except the first letter is 
* Inside the constructor function, we can define the properties that we want each object (in this case, botanic garden) to inherit 
* Along with properties, functions can also be inherited by each object instance. There are two ways we can achieve this:

1. In the constructor function itself 
Example:
```
function Garden(sections, date_opened, admission_fee) {
   this.sections = sections,
   this.date_opened = date_opened,
   this.admission_fee = admission_fee
   this.welcomeVisitor = function() {
       return "Thank you for visiting our garden today!"
   }
} 
garden1.welcomeVisitor // "Thank you for visiting our garden today!"

```
**OR**


2. On the object prototype (preferred method)

```
Garden.prototype.welcomeVisitor = function() {
   return "Thank you for visiting our garden today!"
}
```
