# Domain Modeling ```https://github.com/codefellows/domain_modeling#domain-modeling```

* process of creating a model in code for a specific problem, sometimes called *object-oriented model*

* *object-oriented programming* creates new objects, initializes properties inside the object using *this* as a variable, and stores the object in a variable for later use
```js
var epicFailVideo = function(epicRating, hasAnimals) {
    this.epicRating = epicRating;
    this.hasAnimals = hasAnimals;
}

var parkourFail = new epicFailVideo(7, false);
var corgiFail = new epicFailVideo(4, true);

console.log(parkourFail);
console.log(corgiFail);
```

* Generating random numbers
    * done using ```Math.random()```
    ```js
    var epicFailVideo = function(epicRating, hasAnimals) {
    this.epicRating = epicRating;
    this.hasAnimals = hasAnimals;
    }

    epicFailVideo.prototype.generateRandom = function(min, max) {
        return Math.floor(Math.random() * (max - min +1)) + min;
    }

    var parkourFail = new epicFailVideo(7, false);
    var corgiFail = new epicFailVideo(4, true);

    console.log(parkourFail.generateRandom(1,5));
    console.log(corgiFail.generateRandom(1,5));
    ```

* domain modeling creates a model for a specific problem


# HTML & CSS

## Chapter 6: Tables (p.126-145)

* tables represent information in grid format using the following tags:
    * ```<table>``` establishes a table element
        * ```<tr>``` makes a table row
            * ```<td>``` denotes data that goes in the above row
        * ```<th>``` represents the table heading
    * to span columns use ```<td colspan="2">Geography<td>``` (spans two columns)
    * to span rows use ```<td rowspan="2">```


# Javascript & Jquery

## Chapter 3: Functions, Methods, and Objects (p.106-144)

* the ```+=``` operator is used to add content to an existing variable

* you can add and delete properties by using keywords *add* and *delete*

* arrays are objects that hold a set of key: value pairs but the key for each value is it's index

* the property of any object can hold an array and the value of any element in an array can be an object

* there are three groups of built in objects
    * the browser object model - the topmost object is the browser window
    * the document object model - creates a model of the current web page with the document as the topmost object
    * global javascript objects - dont form a single model but rather a group of objects that relate to different parts of Javascript

* for working with decimal numbers ```.toFixed(3)``` will round the stored number to three decimal places

* ```toPecision(3)``` uses the number in parentheses to indicate the total number of digits the number should have and return the number as a string
