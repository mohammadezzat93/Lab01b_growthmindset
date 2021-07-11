# Table


### What's a Table?

A table represents information in a grid format.
Examples of tables include financial reports, TV
schedules, and sports results.

## Basic Table Structure

**<table>**  
The <table> element is used
to create a table. The contents
of the table are written out row
by row.  
**<tr>**  
You indicate the start of each
row using the opening <tr> tag.
(The tr stands for table row.)
It is followed by one or more<td> elements (one for each cell
in that row).
At the end of the row you use a
closing </tr> tag.  
**<td>**  
Each cell of a table is
represented using a <td>
element. (The td stands for
table data.)  
At the end of each cell you use a
closing </td> tag.  
**<th>**  
The <th> element is used just
like the <td> element but its
purpose is to represent the
heading for either a column or
a row. (The th stands for table
heading.)

## Spanning Column 

- Sometimes you may need the
entries in a table to stretch
across more than one column.
The colspan attribute can be
used on a <th> or <td> element
and indicates how many columns
that cell should run across.

## Spanning Rows

- You may also need entries in
a table to stretch down across
more than one row.
The rowspan attribute can be
used on a <th> or <td> element
to indicate how many rows a cell
should span down the table.

### Example

![Image](https://i.stack.imgur.com/fVgz6.png)

## Long Tables

-There are three elements that
help distinguish between the
main content of the table and
the first and last rows (which can
contain different content).
These elements help people
who use screen readers and also
allow you to style these sections
in a different manner than the
rest of the table .


**<thead>**  
The headings of the table should
sit inside the <thead> element.  
**<tbody>**  
The body should sit inside the <tbody> element.  
**<tfoot>**  
The footer belongs inside the<tfoot> element.  

## Border & Background

- The border attribute was used
on both the <table> and <td>
elements to indicate the width of
the border in pixels.
The bgcolor attribute was used
to indicate background colors
of either the entire table or
individual table cells. 

## Summary TABLES
- The <table> element is used to add tables to a web
page.
- A table is drawn out row by row. Each row is created
with the <tr> element.
- Inside each row there are a number of cells
represented by the <td> element (or <th> if it is a
header).
- You can make cells of a table span more than one row
or column using the rowspan and colspan attributes.
- For long tables you can split the table into a <thead>,
<tbody>, and <tfoot>.

-----------

# Functions, Methods, and Objects

## JavaScript Object Constructors

#### constructor : The constructor method is a special method of a class for creating and initializing an object of that class.

- The **this** Keyword
In JavaScript, the thing called this is the object that "owns" the code.

- The value of this, when used in an object, is the object itself.

- In a constructor function this does not have a value. It is a substitute for the new object. The value of this will become the new object when a new object is created.

- **Note** that this is not a variable. It is a keyword. You cannot change the value of this.  

![Image](https://miro.medium.com/max/1400/1*uO_3V9tJ0ZD0LI-Hi7x2FA.png)


### Adding a Property to a Constructor

- You cannot add a new property to an object constructor the same way you add a new property to an existing object:

- To add a new property to a constructor, you must add it to the constructor function:

#### Example
function Person(first, last, age, eyecolor) {  
  this.firstName = first;  
  this.lastName = last;  
  this.age = age;  
  this.eyeColor = eyecolor;  
  this.nationality = "English";  
}  

## Built-in JavaScript Constructors
### JavaScript has built-in constructors for native objects:

-     new String() // A new String object
-     new Number()    // A new Number object
-     new Boolean()   // A new Boolean object
-     new Object()    // A new Object object
-     new Array()     // A new Array object
-     new RegExp()    // A new RegExp object
-     new Function()  // A new Function object
-     new Date()      // A new Date object

## Arrays of Objects

### What Is An Array Of Objects?

JAVA ARRAY OF OBJECT, as defined by its name, stores an array of objects. Unlike a traditional array that store values like string, integer, Boolean, etc an array of objects stores OBJECTS. The array elements store the location of the reference variables of the object.

### Syntax: 

**Class_Name obj[ ]= new Class_Name[Array_Length];**

**For example**, if you have a class Student, and we want to declare and instantiate an array of Student objects with two objects/object references then it will be written as: 

**Student[ ] studentObjects = new Student[2];**  
And once an array of objects is instantiated like this, then the individual elements of the array of objects needs to be created using the new keyword.

-And once an array of objects is instantiated like this, then the individual elements of the array of objects needs to be created using the new keyword.



- The below figure shows the structure of an Array of Objects :


![Image](https://media.geeksforgeeks.org/wp-content/uploads/20200810184826/arrayofobjects.png)