## Object Literals
A JavaScript object literal is a comma-separated list of name-value pairs wrapped in curly braces. Object literals encapsulate data, enclosing it in a tidy package. This minimizes the use of global variables which can cause problems when combining code.
Object literal property values can be of any data type, including array literals, functions, and nested object literals.
Several JavaScripts from dyn-web use object literals for setup purposes. Object literals enable us to write code that supports lots of features yet still provide a relatively straightforward process for implementers of our code. No need to invoke constructors directly or maintain the correct order of arguments passed to functions. Object literals are also useful for unobtrusive event handling; they can hold the data that would otherwise be passed in function calls from HTML event handler attributes.

There is one drawback: if you are unfamiliar with the syntax, it can be very easy to introduce errors which cause the code to stop working.
### Object Literal Syntax
Object literals are defined using the following syntax rules:

A colon separates property name[1] from value.
A comma separates each name-value pair from the next.
A comma after the last name-value pair is optional.[2]
If any of the syntax rules are broken, such as a missing comma or colon or curly brace, a JavaScript error will be triggered. Browser error messages are helpful in pointing out the general location of object literal syntax errors, but they will not necessarily be completely accurate in pointing out the nature of the error.
[![image](https://xomino.files.wordpress.com/2013/04/j1.png)]

## Document Object Model
The Javascript DOM (Document Object Model) is an interface that allows developers to manipulate the content, structure and style of a website.
This document enables Javascript to access and manipulate the elements and styles of a website. The model is built in a tree structure of objects and defines:
1. HTML elements as objects
2. Properties and events of the HTML elements
3. Methods to access the HTML elements
The places of the elements are referred to as nodes. Not only elements get nodes but also the attributes of elements and text get their own node (attribute-nodes and text-nodes).
The DOM Document is the owner of all other objects in your webpage. That means if you want to access any object on your webpage you always have to start with the document. It also contains many important properties and methods that enable us to access and modify our website.
[![image](https://www.w3schools.com/js/pic_htmltree.gif)]