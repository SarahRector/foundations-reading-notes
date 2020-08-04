# Applying Atomic Design
## Part 1: https://medium.com/backticks-tildes/visually-breaking-down-ui-components-using-atomic-design-part-1-476e1ddd73ca

* Atomic design is a way of thinking about the layout and components of a page
    * **Page** is the page itself
    * **Template** is the page layout without actual content (a skeleton)
    * **Organisims** are large sections that can be easily extracted from the page
    * **Molecules** are sections within an organisim
    * **Atoms** are the basic HTML elements that can't be broken down any further (labels, p tags, etc)

## Part 2: https://medium.com/backticks-tildes/visually-breaking-down-ui-components-using-atomic-design-and-building-with-react-part-2-20eb8aabab4b

* This designer uses a file structure that breaks down components into each atomic stage (one for atoms, molecules, etc)

* When visually breaking down components, start big and work to small, when building, start small and work to bigger things

## The Art of transforming UI features into components
https://theiconic.tech/the-art-of-transforming-ui-features-into-components-e86de5560fd7

* problems with maintaining style guides or pattern libraries because they live outside of the codebase and design tools

* "Ultimately, the key to re-using code and design and thereby the key to consistent user experience as well as rapid development lies in breaking down your features into composable components."

## Thinking in React (only Step 1)
https://reactjs.org/docs/thinking-in-react.html

* start by breaking everything down into a component hierarchy and giving each component names
    * use the *single responsibility principal*

## UI Components By Design
https://www.thoughtworks.com/insights/blog/ui-components-design

* components allow both designers and developers to have a common language to refer to because everything is named

* *foundation components* are typically build by the design team and they ensure a consistent interface and user experience

* *application components* are built by the app team and are usually composed of one or many foundation components

* decouple wherever possible and avoid future-proofing

## Back to Basics: What are Callbacks in JavaScript?
https://www.sitepoint.com/callbacks-javascript/

* a callback is a function that happens after another function has finished executing

## JavaScript Callback Functions
https://www.dashingd3js.com/lessons/javascript-callback-functions

* This article has a great video that explains callback functions

## First-class Function
https://developer.mozilla.org/en-US/docs/Glossary/First-class_Function

* a language has first-class functions if the functions are treated like any other variable (can be passes as arguments, returned by functions or assigned as a value to a variable)
```js
    const foo = function() {
   console.log("foobar");
    }
    // Invoke it using the variable
    foo();
    //We assigned an Anonymous Function in a Variable, then we used that variable to invoke the function by adding parentheses () at the end.
```

## MDN Callback Function
https://developer.mozilla.org/en-US/docs/Glossary/Callback_function

* There are both synchronous and asynchronous callbacks

## JavaScript Classes
https://javascript.info/class

* basic syntax is:
```js
    class User {
        
  constructor(name) {
    this.name = name;
  }

  sayHi() {
    alert(this.name);
  }

    }

    // Usage:
    let user = new User("John");
    user.sayHi();
```

* In JS, a class is a kind of function

## Intro to object-oriented programming in JavaScript: objects, prototypes and classes
https://www.freecodecamp.org/news/an-intro-to-object-oriented-programming-in-javascript-objects-prototypes-and-classes-5d135e7361b1/

* An object is an instance of a class
    * meaning that using a class, you can make objects that al share methods and properties

* Each time you declare a method inside a class, you add that method to the prototype of the corresponding function

## Object Methods, "this"
https://javascript.info/object-methods

* objects represent actual objects in the real world and as such, can *act*. Actions are represented by functions

* "this" is used in methods to represent the object and access a property on it. Ex:
```js
    let user = {
    name: "John",
    age: 30,

    sayHi() {
        // "this" is the "current object"
        alert(this.name);
    }

    };

    user.sayHi(); // John
```
