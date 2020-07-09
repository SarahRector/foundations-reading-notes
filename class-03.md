# HTML & CSS
## Chapter 3: Lists

* Three main types of lists
    * ordered lists ```<ol>``` (numbered)
    * unordered lists ```<ul>``` (bullet points)
    * definition lists ```<dl>``` (series of terms and their definitions)
        * ```<dt>``` is the term being defined
        * ```<dd>``` is the definition
    * can also nest lists inside of each other

## Chapter 13: Boxes

* boxes by default are only sized big enough to hold their contents

* can change using width/height
    * px will measure it by pixel size
    * percentages will measure against browser window or containing box
    * ems will be pased on the size of the text within the box

* can also set min/max width/height to make sure images and text stays within a certain size even as browser window shrinks or expands

* **overflow** tells browser what to do if content is larger than the box itself
    * *hidden* hides whatever doesn't fit
    * *scroll* adds a scrollbar to the box

* every box has three properties: *border, padding and margin*
    * **border** is the actual line that seperates one box from another
    * **margin** is the space outside of the border 
        * if width is specified then margin is added to the width
    * **padding** is the space inside of the border
        * if width is specified for a box, padding is added to the width of the box

* border can be styled in many ways
    * border-width: sets width
    * border-style: allows you to choose what it looks like (solid, dotted, dashed, double, groove, ridge, inset, etc)
    * border-color: changes color
    * can all be written in shorthand as ```border: 5px dotted yellow```

* to center a box on the page you can set the left and right margin to auto
    * for this to work you must set a width for the box
    * if you don't want the text in the box to be centered you need to specify ```text-align: left```

* can hide boxes using ```visibility: hidden```

* can use images for borders by using ```border-image: url('this is the url')11 11 11 11 round;```etc

* can create box shadows by using ```box-shadow``` and then using a box-shadow generator

* rounded cornder can be made using ```border-radius```


# Javascript & Jquery

## Decisions and Loops (p.162 - 182)

* switch statements
    * starts with *switch value* and then indicates possible values and which code that should run if the variable matches that value
    * switch statements end with *break* which tells computer to stop and move on to other code
    ```js
    switch (level) {
        case 'One':
            title = 'Level 1';
            break;
        case 'Two':
            title = 'Level 2';
            break;
    }
    ```
* **loops** check a condition and if it's true, it runs the code block and then keep checking it if it still returns true
* three main types of loops
    * *for* loops: runs for a specified number of times
    ```js
    for (i = 0; i < 10; i++>) {
        document.write(i);
    }
    ```
    It *initializes* ```i = 0```
    Then sets a condition ```i < 10```
    Then updates ```i++```

    * *while* loops can have a condition other than a counter and the code will keep looping whild the condition is still true

    * *do while* loops run the condition inside the curly braces at least once, even if the condition is false