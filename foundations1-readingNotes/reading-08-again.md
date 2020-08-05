# HTML & CSS
## Chapter 15: Layout (p.360 - 402)

* block-level elements: start on a new line (h1, p, ul, li elements)
* inline-elements: flow in between surrounding text (img, b, i elements)
* containing elements: contain the elements within them (divs)
* *positioning* in CSS means that things are positioned relative to other things.
    * normal flow (default) means that each block-level element sits on top of each other
    * relative positioning moves an element relative to where it would have been in normal flow
    * absolute positioning moves an element in relation to the containing element
    * fixed positioning positions an element in relation to the browser
* *z-index* controls overlapping elements by assinging them a value.  The higher the value, the closer the element is to the top in relation to the other elements
* *float* allows you to float an element as far to the right or left of it's containing element as possible
    * can use float to create multiple columns by creating a div element for each column (see pg 375)
* you can have multiple style sheets but you have to link them in the HTML or import them all to one stylesheet that then links to the HTML