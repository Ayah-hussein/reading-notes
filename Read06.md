The HTML tables allow web authors to arrange data like text, images, links, other tables, etc. into rows and columns of cells.

The HTML tables are created using the `<table>` tag in which the `<tr>` tag is used to create table rows and `<td>` tag is used to create data cells. The elements under `<td>` are regular and left aligned by default.
**Ex**
 < !DOCTYPE html>
< html>

   < head>
      < title>HTML Table Cellpadding< /title>
   < /head>
	
   < body>
      < table border = "1" cellpadding = "5" cellspacing = "5">
        < tr>
            < th>Name</ th>
            < th>Salary< /th>
         < /tr>
         < tr>
            < td>Ramesh Raman </ td>
            < td>5000</ td>
         </ tr>
         < tr>
            < td>Shabbir Hussein </ td>
            < td>7000</ td>
         < /tr>
      < /table>
   </ body>
	
</ html> 

## Objects and properties
A JavaScript object has properties associated with it. A property of an object can be explained as a variable that is attached to the object. Object properties are basically the same as ordinary JavaScript variables, except for the attachment to objects. The properties of an object define the characteristics of the object. You access the properties of an object with a simple dot-notation:

objectName.propertyName

object initializer, which is a comma-delimited list of zero or more pairs of property names and associated values of an object, enclosed in curly braces ({}):

var myCar = {
    make: 'Ford',
    model: 'Mustang',
    year: 1969
};


## Defining methods
A method is a function associated with an object, or, put differently, a method is a property of an object that is a function. Methods are defined the way normal functions are defined, except that they have to be assigned as the property of an object. See also method definitions for more details. An example is:

**objectName.methodname = functionName;**

var myObj = {
  myMethod: function(params) {
    // ...do something
  }

  // OR THIS WORKS TOO

  myOtherMethod(params) {
    // ...do something else
  }
};
where objectName is an existing object, methodname is the name you are assigning to the method, and functionName is the name of the function.

- You can then call the method in the context of the object as follows:

object.methodname(params);

### Using this for object references
JavaScript has a special keyword, this, that you can use within a method to refer to the current object. For example, suppose you have 2 objects, Managerand Intern. Each object have their own name, age and job.  In the function sayHi(), notice there is this.name. When added to the 2 objects they can be called and returns the 'Hello, My name is' then adds the name value from that specific object. As shown below. 

const Manager = {
  name: "John",
  age: 27,
  job: "Software Engineer"
}
const Intern= {
  name: "Ben",
  age: 21,
  job: "Software Engineer Intern"
}

function sayHi() {
    console.log('Hello, my name is', this.name)
}

// add sayHi function to both objects
Manager.sayHi = sayHi;
Intern.sayHi = sayHi;

Manager.sayHi() // Hello, my name is John'
Intern.sayHi() // Hello, my name is Ben'
The this refers to the object that it is in. You can create a new function called howOldAmI()which logs a sentence saying how old the person is. 

function howOldAmI (){
  console.log('I am ' + this.age + ' years old.')
}
Manager.howOldAmI = howOldAmI;
Manager.howOldAmI() // I am 27 years old.


 ## function
  is a group of reusable code which can be called anywhere in your program. This eliminates the need of writing the same code again and again. It helps programmers in writing modular codes. Functions allow a programmer to divide a big program into a number of small and manageable functions.

Like any other advanced programming language, JavaScript also supports all the features necessary to write modular code using functions. You must have seen functions like alert() and write() in the earlier chapters. We were using these functions again and again, but they had been written in core JavaScript only once.

JavaScript allows us to write our own functions as well. This section explains how to write your own functions in JavaScript.

Function Definition
Before we use a function, we need to define it. The most common way to define a function in JavaScript is by using the function keyword, followed by a unique function name, a list of parameters (that might be empty), and a statement block surrounded by curly braces.

Syntax
The basic syntax is shown here.

< script type = "text/javascript">
   <!--
      function functionname(parameter-list) {
         statements
      }
   //-->
< /script>
Example
Try the following example. It defines a function called sayHello that takes no parameters −

< script type = "text/javascript">
   <!--
      function sayHello() {
         alert("Hello there");
      }
   //-->
< /script>

**Calling a Function**
To invoke a function somewhere later in the script, you would simply need to write the name of that function as shown in the following code.

**Ex:**
< html>
   < head>   
      < script type = "text/javascript">
         function sayHello() {
            document.write ("Hello there!");
         }
      < /script>
      
   < /head>
   
   < body>
      < p>Click the following button to call the function< /p>      
      < form>
         < input type = "button" onclick = "sayHello()" value = "Say Hello">
      < /form>      
      < p>Use different text in write method and then try...< /p>
   </ body>
</ html>
