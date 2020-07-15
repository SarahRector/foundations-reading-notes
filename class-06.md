# Javascript & Jquery

## Chapter 3: Object Literals (p.100 - 105)
* An object is a group of variables and functions to try to represent something from the real world
    * variables are known as *properties*
    * functions are known as *methods*
    * they are grouped together in *key: value pairs*

* objects are created using *literal notation* - all of the key: value pairs and methods are spelled out in the body of the object

* objects can be accessed using *dot notation*
    ```const hotelName = hotel.name;```

## Chapter 5: Document Object Model (p. 183 - 242)
* you can both access and update the DOM using a variety of properties
    * getElementById, querySelector (accesses 1st matching element), querySelectorAll(gets all matching elements, getElementByClassName), etc

* you can work with those elements using a variety of methods or properties
    * nodeValue, innerHTML, textContent, createElement(), append, etc

* can use either *item() method* or array syntax to access a node from a node list but array syntax is preferred
    
```js
    const elements = document.getElementByClassName('hot);
    if (elements.length >= 1) {
        var firstItem = elements[0];
    }
```

* getElementsByClassName() returns a nodelist of elements with a matching class name
* getElementsByTagName() allows you to select items using their tag name
* querySelector() uses a CSS selector as its parameter

* you can loop through a node list to change the value of each element
    * have to know the length of the list (using .length)

* to access and change a text node you have to get it, get it's text content, and then change the text content and value
    
* *innerHTML* will get the content of and element and return it as one long string

* for example, a shopping list, you could add things to the list by using the following:
```js
var newEl = document.createElement('li'); //stores the new element in a variable
var newText = document.createTextNode('quinoa'); //creates new text conent for that variable
newEl.appendChild(newText); //attatches the new text to the new element
var position = document.getElementByTagName('ul')[0]; //finds the position where we are adding new element
position.appendChild(newEl); //inserts the new element
```
* cross-site scripting attacks (xss) happen when attackers place malicious code into a site
    * prevent by only allowing type of characters needed for user input. Known as *validation*
