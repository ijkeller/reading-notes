## Readings: Problem Domain, Objects, and the DOM

### [JavaScript Object Basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)

How would you describe an object to a non-technical friend you grew up with?

- a set of items and actions that are grouped together for some purpose, like enemies on a video game, they all have certain attributes like type, size, attacks, etc

What are some advantages to creating object literals?

- easily encapsulate data in a manageable package,
- minimizes the use of global variables which can cause problems when combining code

How do objects differ from arrays?

- Arrays are objects who's key in the key-value pair is the index number

Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.

- when you need to access object properties using variable

Evaluate the code below. What does the term <span style="color:#990000">**this**</span> refer to and what is the advantage to using <span style="color:#990000">**this**</span>?

```js
const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}
```

- <span style="color:#990000">**this**</span> is the instance of the object being called.  Allows you to write a function (method) for each individual instance of an object.

----------------

### [Introduction To The DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)

What is the DOM?

- Document Object Model, a programming interface for web documents

Briefly describe the relationship between the DOM and JavaScript.

- allows javascript to access and manipulate the webpage

What’s the difference between primitive values and object references in JavaScript?

- primitive values are basic types of information like numbers, strings, or booleans
- reference values are more complicated sets of data like objects, arrays, or functions.

----------------------

## Things I want to know more about

- sdf
