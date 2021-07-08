

## Object Literals

**A JavaScript object literal** is a comma-separated list of name-value pairs wrapped in curly braces. Object literals encapsulate data, enclosing it in a tidy package. This minimizes the use of global variables which can cause problems when combining code.

- The following demonstrates an example object literal:

**var myObject = {  
    sProp: 'some string value',  
    numProp: 2,  
    bProp: false  
};  **

- Object literal property values can be of any data type, including array literals, functions, and nested object literals. 

- Those values can be properties and functions. Here’s a snippet of an object literal with one property and one function.  

**var greeting = {  
    fullname: "Michael Jackson",  
    greet: (message, name) => {  
        console.log(message + " " + name + "!!");  
    }  
};** 

Here’s the snippet to use the object we just created to log the fullname and call the greet function with the fullname value.

*//log fullname  
console.log(greeting.fullname);  
//call greet function  
greeting.greet("Greeting", greeting.fullname);  
---------------output----------------  
Michael Jackson  
Greeting Michael Jackson!!  *

--------------------

## Document Object Model

### The HTML DOM (Document Object Model)

- When a web page is loaded, the browser creates a Document Object Model of the page.

-The HTML DOM model is constructed as a tree of Objects:

                        The HTML DOM Tree of Objects

![Image](https://1.bp.blogspot.com/-Z0QnE9eWAnM/XWj6B0TmfmI/AAAAAAAAZps/aRfAU517hg0ovfzgLUTZkmjHD3SXZCoWACLcBGAs/s1600/DOM.PNG)  

- With the object model, JavaScript gets all the power it needs to create dynamic HTML:

• JavaScript can change all the HTML elements in the page  
• JavaScript can change all the HTML attributes in the page  
• JavaScript can change all the CSS styles in the page  
• JavaScript can remove existing HTML elements and attributes  
• JavaScript can add new HTML elements and attributes  
• JavaScript can react to all existing HTML events in the page  
• JavaScript can create new HTML events in the page  

- The document object represents your web page.

-If you want to access any element in an HTML page, you always start with accessing the document object.

-Below are some examples of how you can use the document object to access and manipulate HTML.

| Method | Description 
| :---: | :---:
| document.getElementById(id) | element by element id 
| document.getElementsByTagName(name) | Find elements by tag name
| document.getElementsByClassName(name) | Find elements by class name


### Adding and Deleting Elements

| Method | Description 
| :---: | :---:
| document.createElement(element) | Create an HTML element
| document.removeChild(element) | Remove an HTML element
| document.appendChild(element) | Add an HTML element
| document.replaceChild(new, old) | Replace an HTML element
| document.write(text) | Write into the HTML output stream
	
---------------

### Understanding the problem domain is the hardest part of programming

- Understanding The Problem Domain Is The Hardest Part Of Programming
What is the hardest thing about writing code?

-There are many common answers to this question:

• Learning a new technology  
• Naming things    
• Testing your code  
• Debugging  
• Fixing bugs  
• Making software maintainable  

### Why problem domains are hard

- The big issue is that many problem domains are like a puzzle with a blurry picture or no picture at all.
The real world is a messy place.  Many of the problem domains we face as programmers are difficult to understand and look completely different depending on your viewpoint.  

- As programmers, we also are often not given complete information about the problem domain, so we don’t even have the information we need to understand it.

### What can you do about it?
- If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:

- Make the problem domain easier
Get better at understanding the problem domain
You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.

- What I mean by this is that it is often beneficial to take a part of the problem and fully understand that part before expanding the problem domain.


	
	
	