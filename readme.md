1. **Write a blog on Difference between HTTP1.1 vs HTTP2**

   Find the Blog link:link:=>https://medium.com/@velsabari66/1-differences-between-http-1-1-and-http-2-e32e15a71474


2. **Write a blog about objects and its internal representation in Javascript**
     
##Introduction:
                JavaScript, the programming language that powers the dynamic behavior of the web, is renowned for its versatile and powerful object-oriented features. Objects play a central role in JavaScript, serving as the building blocks for data structures and enabling developers to model real-world entities. In this blog, we'll explore the concept of objects in JavaScript and delve into their internal representation.
    

The Basics of Objects in JavaScript:
                 In JavaScript, an object is a composite data type that allows you to group related data and functions together. Objects are instances of a class, and they can be created using either literal notation or the Object constructor. Here's a simple example:
                    
                 const person = {
                 firstName: 'Sabari',
                 lastName: 'vel',
                 age: 22,
                 sayHello: function() {
                 console.log('Hello!');
                  }

In this example, person is an object with properties (`firstName``, `lastName``, `age``) and a method (`sayHello``). The properties can be accessed using dot notation (`person.firstName``) or bracket notation (`person['firstName']``).

Internal Representation of Objects:
                 Internally, JavaScript engines use various mechanisms to represent objects. One common representation is the property map, a data structure that associates property names with values. Each object has a hidden property map that stores its properties and their corresponding values.

Reference to the Prototype:
                 JavaScript follows a prototype-based inheritance model. Objects can inherit properties and methods from other objects known as prototypes. The internal representation includes a reference to the prototype of the object, forming a prototype chain.

// Creating a prototype object
const personPrototype = {
  sayGreeting: function() {
    console.log('Greetings!');
  }
};


const person = Object.create(personPrototype);
person.firstName = 'Sabari';
person.lastName = 'vel';
person.age = 22;

person.sayGreeting(); // Outputs: Greetings!
 
 In this example, `person `inherits the `sayGreeting `method from `personPrototype`.
  
Property Descriptors:
                Each property in an object has an associated property descriptor that defines its behavior. Property descriptors include information about whether the property is writable, enumerable, and configurable. You can access property descriptors using the `Object.getOwnPropertyDescriptor`method.
                const obj = { name: 'Example' };

const descriptor = Object.getOwnPropertyDescriptor(obj, 'name');
console.log(descriptor);
// Outputs: { value: 'Example', writable: true, enumerable: true, configurable: true }

Memory Management:
                JavaScript engines handle memory management for objects. They use garbage collection to automatically reclaim memory occupied by objects that are no longer reachable. Developers need not explicitly manage memory allocation and deallocation.

Conclusion:
           Understanding the internal representation of objects in JavaScript is crucial for writing efficient and maintainable code. Objects, with their versatile capabilities and internal mechanisms, empower developers to create complex applications with ease. As you delve deeper into JavaScript development, a solid grasp of object-oriented concepts will undoubtedly enhance your coding skills and enable you to build robust and scalable applications.
 

