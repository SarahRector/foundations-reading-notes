# MDN Template Literals (template strings)
## https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals

* Syntax
```js
    `string text`

    `string text line 1
     string text line 2`

    `string text ${expression} string text`

    tag`string text ${expression} string text`
```
* enclosed by backticks and can contain **placeholders** which are indicated by dollar sign and curly braces ```(${expression})```
    * the egpression in the placeholder and the text between the backticks get passed to a function
    * default function concatenates the parts into a single string

* using template literals you can have multi line strings by using backticks
* this allows you to make code more readable. ex:
    ```js
    let a = 5;
    let b = 10;
    console.log(`Fifteen is ${a + b} and
    not ${2 * a + b}.`);
    // "Fifteen is 15 and
    // not 20."
    ```
* **string.raw** allows ou to create raw strings

# Getting Literal With ES6 Template Strings
## https://developers.google.com/web/updates/2015/01/ES6-Template-Strings

* template strings allow us to take any valid java script expression and inside a template literal, the result will be output as part of the same string.

* ```js
    // Simple string substitution
    var name = "Brendan";
    console.log(`Yo, ${name}!`);

    // => "Yo, Brendan!"

    //using expression interpolation to embed readable inline math
    var a = 10;
    var b = 10;
    console.log(`JavaScript first appeared ${a+b} years ago. Wow!`);

    //=> JavaScript first appeared 20 years ago. Wow!

    console.log(`The number of JS MVC frameworks is ${2 * (a + b)} and not ${10 * (a + b)}.`);
    //=> The number of JS frameworks is 40 and not 200.

    //or for functions inside of expressions
    function fn() { return "I am a result. Rarr"; }
    console.log(`foo ${fn()} bar`);
    //=> foo I am a result. Rarr bar.
    ```
* any whitespace inside of backtick syntax will also be considered part of the string

* tagged templates transform a template string by placing a function name before the template string

# Template Literals (from CSS-Tricks)
## https://css-tricks.com/template-literals/

* **expressions** allow us to put a value in a string. ex:
    ```js
    let name = `Ryan`;
    console.log(`Hi my name is ${name});
    //returns `Hi my name is Ryan`
    ```

* can also use template literals/strings to create templates for data in javaScript

# MDN forEach
## https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach

* **forEach** is a method that executes a function once for each element in an array. ex:
```js
    const array1 = ['a', 'b', 'c'];

    array1.forEach(element => console.log(element));

    // expected output: "a"
    // expected output: "b"
    // expected output: "c"
```
* **Syntax** ```arr.forEach(callback(currentValue [, index [, array]])[, thisArg])```

# For loops vs forEach in JavaScript
## https://medium.com/@abustamam/for-loops-vs-foreach-in-javascript-7a977278a39e

* forEach does a similar thing to a for loop but is easier to read because it's closer to actual English

* these do the same thing:
```js
    for (var i = 0; i < arr.length; i++) {
    console.log('Element', i, 'is', arr[i]);
    }
    arr.forEach(function(element, i) {
    console.log('Element', i, 'is', element);
    });
```
* forEach only works on arrays, so if you want to *count* something, for looks are better







