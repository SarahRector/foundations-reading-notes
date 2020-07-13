# HTML & CSS
## Chapter 4: Links

* created using the ```<a>``` element
```<a href="http://www.imdb.com">IMDB</a>```

* to link to other pages on the same site you can use a *relative url*
    * ex: ```<a href = "index.html>Home</a>``` this returns user to the home page

* to generate a link that will start the users email program use ```<a href = "mailto:chickypickle@gmail.com>Email</a>```

* to have your link open in a new window use *target*
```js
<a href = "http://www.imdb.com" target="_blank">IMDB</a>
```
* to link to a different part of the page you are on (like to go from the top of the page to the bottom of the page) the parts of the page you want to link to must have an id in HTML. Then link as follows:
```js
<h1 id = "top">Film Making Terms</h1>
<a href = "#top">Top</a>
```


## Chapter 15: Layout

* Normal flow is default
* *position: relative* moves an element to where it would have been in normal flow
    * you can then use offset properites (top, bottom, left, right) to move the item from where it would have been in normal flow

* *position: absolute* takes the parent box out of the equation and moves elements relative to the edge of the screen

* *position: fixed* fixes an element relative to the browser window and allows other parts of the page to scroll under it

* if boxes overlap, use *z-index: 10;* which makes that box the priotiry and displays it on top

* *float: right;* takes an element in normal flow and allows you to move it to the left or the right.  Other items on the page will flow around it

* Can also use floats to create columns

* *fixed width layouts* are measured in pixels and stay fixes, *liquid layouts* expand and contract with the browser window and usually are reasured in percentages

* sometimes pages have multiple stylesheets, which can be linked in different ways
    * have one main stylesheet that imports the other stylesheets using ```@import url("tables.css");```
    * put links to all of your stylesheets in the head of your HTML

# Javascript and Jquery
## Chapter 3: Functions, Methods and Objects (p.86-99)

* functions let you group a bunch of statements together to perform a task

* to *declare* a function you have to name it and then write instructions for it inside of curly braces
```js
function sayHello() {
    document.write('Hello');
}
```
* once you have a function declared, you can use it by *calling* it ```sayHello();```

* sometimes, when you declare a function, it needs information to work so you have to set *paramaters*
```js
function getArea(width, height) {
    return width * height;
}
```

* when calling a function with paramaters, you have to specify the values of those paramaters after its name.  These can be actual values or variables.
```js
wallWidth = 3;
wallHeight = 5;
getArea(wallWidth, wallHeight);
```
* variables can be *local* (called within that function) or *global* (called outside of the function so accessible to many functions)


# Article
## "6 reasons for pair programming"

* Greater Efficiency
    * you would think it takes way longer when it actually takes about the same time and produces higher quality, cleaner code

* Engaged Collaboration
    * when two people are working together they are more engaged and can help each other problem solve

* Learning from Fellow Students
    * everyone has different skill sets and pair programming allows people to get new perspectives and think about solving problems ways that they might not have

* Social Skills
    * good programming is great but no one wants to work with someone who can't work well with others

* Job Interview Readiness
    * coding is part of the job interview process, so it's good to get used to doing it with other people and to practice explaining what youre doing and why

* Work Environment Readiness
    * coding usually happens in teams, if you are already familiar to working this way, that's one less hurdle to overcomesum$