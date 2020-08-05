# HTML & CSS
## Chapter 2: Text
* Headings
    * have six levels (h1 - h6)
    * h1 is main headings
    * h2 is subheadings
    * h1 is hargest, h6 smallest

* Paragraphs
    * default shows each paragraph on a new line
    ```<p></p>```

* Bold and Italic
    * can be done inline
    ```js
    <b>This text is bold</b>
    -or-
    <i>This text is italic</i>
    ```

* Subscript and Superscript

    ```<p>On the 4<sup>th</sup> of September...The amount of CO<sub>2</sub>in the air```

* White Space Collapsing
    * browser collapses any spaces, indents, or line breaks in text into one space

* Line Breaks and Horizontal Rules
    * to get a line break in the middle of a paragraph or between elements use ```<br>```
    * to get a horizontal line (rule) use ```<hr>```

* Strong and Emphasis
    * ```<strong></strong>``` defaults to **bold** in a browser
    * ```<em>```(emphasis) defaults to *italic* in a browser

* Quotations
    * ```<blockquote></blockquote>``` wraps a ```<p></p>``` and will normally be indented. Used for large blocks of text.
    *```<q></q>``` is used for shorter quotes in a paragraph

* Address
    * Contains contact details for the author of the page
    ```js
    <address>
        <p><a href="mailto:homer@example.org">homer@example.org</a></p>
        <p>742 Evergreen Terrace, Springfield</p>
    </address>
    ```

## Chapter 10: Introducing CSS
    
* CSS associates rules with HTML elements

* it does that using *selectors*
    * Indicates the HTML element that the rule applies to
* and *declarations*
    * tells how to style the element
    * are inside curly brackets and also contain a *value*
        * value specifies the settings of the declaration

* *selectors* allow you to target specific elements in an HTML doc
    * are case senitive and must match element exactly

* CSS rules cascade so if two selectors are identical, the last rule will govern
    * also takes into account specificity so if one selector is more specific, it will govern

* building an external (to HTML) style sheet allows you to share styling across multiple elements without duplicating work

# Javascript & Jquery

## Chapter 2: Basic Javascript

* Each individual Javascript instruction is a *statement*
    * each one starts on a new line and ends with a semicolon
    * can be organized into *code blocks* by enclosing instructions in { }

* Comments should be included to explain what your code does

* Information that the computer needs to do it's job (calculations, remember a name, etc) are stored as *variables*

* Data types include:
    * Numbers (actual numbers)
    * Strings ('This string has words and numbers 49858')
    * Booleans (have values of only true or false)

* Variables are declared and are assigned values in the same statement

* Once a variable has been assigned, you can then change what is stored in the variable by using ```variable name = new thing```

* *Arrays* are special variables that stores a list of values
    * can add or remove values from an array
    * also must be named
    * values in an array don't need to be the same data type (can include number, string, boolean)
    * values are accessed like in a numbered list with the 1st position being 0
    * *operators* let you create one value from multiple values
        * ex: ```area = 3 * 2``` (is an arithmetic operator)

## Chapter 4: Decisions and Loops (p. 145 - 162)

* Throughout code there are places where decisions must be made on which code runs
    * to determine what code runs yu set a *condition* then you evaluate that condition
    * can do this using *comparison operators*
* the operands do not have to be only single values.  They can be expessions because the expression will evaluate to a single value
* *logical operators* let you compare the results of more than one comparison
    * ex: ```&& (and) || (or) ! (not)```
* *if statements* check if the condition in a statement evaluates to true.  If it does, then it runs whatever code is next.