# Articles about CSS transitions and animation

## https://learn.shayhowe.com/advanced-html-css/css-transforms/

* *transform* property can be either 2D or 3D
    * 2D: works on x and y axis
    * **rotate** can rotate by degrees
        * default point of the rotation is the center of the element
    * **scale** changes the size of the element
        * default is 1 so less than one makes it smaller and more than one makes it bigger
        * can scale height, width, or height and width at the same time by using x and y simultaneously
    * **translate** pushes and pulls and element in different directions
        * **translateX** changes value on x axis, **translateY** changes value on y axis
    * **skew** distorts x, y or both

    * can combine multiple transforms not with declarations, but by adding properties

    * **transform-origin** can change the origin from the default of center so somewhere else

    * can also change perspective

    * many of these transforms are also available in 3d but with more values as it uses x, y and z axes


    ## https://learn.shayhowe.com/advanced-html-css/transitions-animations/

    * can make animations in CSS and HTMl using certain pseudo-classes like *:hover, :focus, :active, and :target*

    * also use four transition related properties: *transition-property, transition-duration, transition-timing-function and transformation-delay*
        * can transition almost any CSS property (color, font size, etc)

    * can animate using ```@keyframes```
        * this is also extremely complicated and this article provides great instructions for how to get started


## http://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users

* **fade in** sets inital state and then the state of the change, ex: opacity

* **change color**
    ```js
    .color:hover
        {
            background:#53a7ea;
        }
    ```

* **grow and shrink** uses **transform** to grow or shrink something

* **rotate elements** rotates elements on the z axis

* **square to circle** turns a square to a circle and vice-versa

* **3D shadow** adds box shadow and then moves it

* **swing** moves and element left and right

* **inset border** makes an inset box shadow


## https://codepen.io/retyui/pen/ByoaXV

* examples of some buttons

## https://codepen.io/akshaychauhan/pen/oAfae

* keyframes animations examples

## https://codepen.io/kieranfivestars/pen/MYdQxX

* transforming and rotating, etc keyframes animation example

## https://codepen.io/dp_lewis/pen/gCfBv

* square to circle bounce animation

