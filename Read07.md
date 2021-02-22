# HTML Tables

The HTML tables allow web authors to arrange data like text, images, links, other tables, etc. into rows and columns of cells.

The HTML tables are created using the `<table>` tag in which the `<tr>` tag is used to create table rows and `<td>` tag is used to create data cells. The elements under `<td>` are regular and left aligned by default.


## JavaScript constructor functions
 how to use the object literal syntax to create a new object:

let person = {
    firstName: 'John',
    lastName: 'Doe'
};
- Code language: JavaScript (javascript)
In practice, you often need to create many similar objects like a list of persons.

To do this, you can use a constructor function to define a custom type and the new operator to create multiple objects from this type.

Technically speaking, a constructor function is a regular function with the following convention:

- the name of a constructor function starts with a capital letter like Person, Document, etc.
- A constructor function should be called only with the new operator.
Note that ES6 introduces the class keyword that allows you to define a custom type. And classes are just syntactic sugar over the constructor functions with some enhancements.

***The following example defines a constructor function called Person:***

function Person(firstName, lastName) {
    this.firstName = firstName;
    this.lastName = lastName;
}
**Code language: JavaScript (javascript)**
As you can see, the Person is the same as a regular function except that its name starts with the capital letter P.

- To create a new instance of the Person, you use the new operator:

let person = new Person('John','Doe');
Code language: JavaScript (javascript)
Basically, the new operator does the following:

- Create a new empty object and assign it to this.
Assign the arguments 'John' and 'Doe' to the firstName and lastName properties.

Return the this value.
It’s functionally equivalent to the following:

function Person(firstName, lastName) {
    // this = {};

    // add properties to this
    this.firstName = firstName;
    this.lastName = lastName;

    // return this;
}
- Code language: JavaScript (javascript)
Therefore, the following statement:

let person = new Person('John','Doe');
Code language: JavaScript (javascript)
… returns the same result as the following statement:

let person = {
    firstName: 'John',
    lastName: 'Doe'
};
Code language: JavaScript (javascript)
However, the constructor function Person allows you to create multiple similar objects. For example:

let person1 = new Person('Jane','Doe')
let person2 = new Person('James','Smith')
Code language: JavaScript (javascript)
Adding methods to JavaScript constructor functions
An object may have methods that manipulate its data. To add a method to an object created via the constructor function, you can use the this keyword. For example:

function Person(firstName, lastName) {
    this.firstName = firstName;
    this.lastName = lastName;

    this.getFullName = function () {
        return this.firstName + " " + this.lastName;
    };
}

Now, you can create a new Person object and invoke the getFullName() method:

let person = new Person("John", "Doe");
console.log(person.getFullName());

Output:

John Doe
The problem with the constructor function is that when you create multiple instances of the Person, the this.getFullName() is duplicated in every instance. This is not memory efficient.

To resolve this, you can use the prototype so that all instances of a custom type can share the same method.

Returning from constructor functions
Typically, a constructor function implicitly returns this that set to the newly created object. But if it has a return statement, then here’s the rule:

If return is called with an object, the constructor function returns that object instead of this.
If return is called with a value other than an object, it’s ignored.
Calling a constructor function without the new keyword
It’s possible to call a constructor function without the new keyword like this:

let person = Person('John','Doe');
Code language: JavaScript (javascript)
In this case, the Person just executes like a regular function. Therefore, the this inside the Person function doesn’t bound to the person variable but the global object.

If you attempt to access the firstName or lastName property, you’ll get an error:

console.log(person.firstName);
Code language: CSS (css)
Error:

TypeError: Cannot read property 'firstName' of undefined
Code language: JavaScript (javascript)
Similarly, you cannot access the getFullName() method since it’s bound to the global object.

person.getFullName();
Code language: CSS (css)
Error:

TypeError: Cannot read property 'getFullName' of undefined
Code language: JavaScript (javascript)
To prevent a constructor function to be invoked without the new keyword, ES6 introduced the new.target property.

If a constructor function is called with the new keyword, the new.target returns a reference to the function. Otherwise, it returns undefined.

Let’s show the value of the new.target to the console inside the Person function:

function Person(firstName, lastName) {
    console.log(new.target);

    this.firstName = firstName;
    this.lastName = lastName;

    this.getFullName = function () {
        return this.firstName + " " + this.lastName;
    };
}

The following returns undefined because the Person constructor function is called like a regular function:

let person = Person("John", "Doe");

Output:

undefined

However, the following returns a reference to the Person function because it’s called with the new keyword:

let person = new Person("John", "Doe");

Output:

[Function: Person]
Code language: JSON / JSON with Comments (json)
By leveraging the new.target, you can force users of the constructor function to call it with the new keyword. And you can throw an error if they don’t do so like this:

function Person(firstName, lastName) {
    if (!new.target) {
        throw Error("Cannot be called without the new keyword");
    }

    this.firstName = firstName;
    this.lastName = lastName;
}