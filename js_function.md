# Functions in javascript:

Programmers use functions, methods, and objects to organize their code.

## Functions: consist of a series of statements that have been grouped together because they perform a specific task.

### WHAT IS A FUNCTION?
Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of st atements).

*example:*
var msg = 'Sign up to receive our newsletter for 10% off!';
function updateMessage() {
var el = document.getElementByld('message'};
el .textContent = msg;
}
updateMessage(};

*A JavaScript function is executed when "something" invokes it (calls it)*.*

**Function syntax:**

function name(parameter1, parameter2, parameter3) {
  // code to be executed
}

**Function Invocation**
The code inside the function will execute when "something" invokes (calls) the function:

When an event occurs (when a user clicks a button)
When it is invoked (called) from JavaScript code
Automatically (self invoked)

***Why Functions?***

You can reuse code: Define the code once, and use it many times.

You can use the same code many times with different arguments, to produce different results.

Accessing a function without () will return the function object instead of the function result>

 *ex:* 
function toCelsius(fahrenheit) {
  return (5/9) * (fahrenheit-32);
}
document.getElementById("demo").innerHTML = toCelsius;