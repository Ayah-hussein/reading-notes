# The object literal 
The object literal is one of the most popular patterns for creating objects in JavaScript because of its simplicity. ES6 makes the object literal more succinct and powerful by extending the syntax in some ways.

**Object property initializer shorthand**
Prior to ES6, an object literal is a collection of name-value pairs. For example:

function createMachine(name, status) {
    return {
        name: name,
        status: status
    };
}

**JavaScript** is a prototype based language, so everything is an ***object***. It is a must that language to provide easy constructs when it comes to objects creation, configuration and accessing prototypes.

- It’s a common task to define an object and setup it’s prototype. I always felt that setting up the prototype should be allowed directly in the object literal, using a single statement.

- Unfortunately the limitations of the literal didn’t allow to achieve that with a straightforward solution. You had to use Object.create() in combination with the object literal to setup the prototype:

var myProto = {
  propertyExists: function(name) {
    return name in this;
  },
};
var myNumbers = Object.create(myProto);
myNumbers['array'] = [1, 6, 7];
myNumbers.propertyExists('array'); // => true
myNumbers.propertyExists('collection'); // => false

## JS DOM
***The Document Object Model***, or the **“DOM”**, defines the logical structure of HTML documents & essentially acts as an interface to web pages. Through the use of programming languages such as JavaScript, we can access the DOM to manipulate websites and make them interactive.
In this article we’re going to be working with the document object, taking a look at the DOM tree and nodes, and we’ll learn all about how to access and work with elements.



**What is the DOM?**

At its core a website must consist of an HTML document, an index.html. Using a browser we view the website, which renders from our HTML file/s and any CSS files which add style and layout rules.


The browser also creates a representation of this document known as the Document Object Model. It’s through the use of the DOM, that JavaScript is able to access and alter the content and elements of the website.
To view the DOM, using your web browser, right click anywhere on a page and choose “Inspect”. This will open up Developer Tools.

***The Document Object***
The document object is a built-in object, containing many properties and methods.
We access and manipulate this object with JavaScript. And by manipulating the DOM, we can now make our web pages highly interactive! As we’re no longer limited to just building static sites with styled HTML content.

**The DOM Tree & Nodes**
Largely due to the layout of the DOM, it’s often called the DOM Tree:

![domtree](domtree.png)
