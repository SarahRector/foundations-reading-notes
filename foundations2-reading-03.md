# Responsive Web Design
https://learn.shayhowe.com/advanced-html-css/responsive-web-design/

* responsive web design means that the website looks good and works on every device and screen

* broken down into three main components
    * flexible layouts
        * use a flexible grid that dynamically resizes (uses em units or percentages)
    * media queries
        * specify different styles for individual browser and devices
        * can do this using **@media** or **@import**
        * have three logical operators: and, not and only
        * can also specify resolution, orientation, aspect-ratio and height/width
        * can also use viewport to help display on mobile devices
    * flexible media
        * can make media (img, video, canvas, etc) flexible by using max-width: 100%
            * max-width doesn't work with iframes

# All About Floats
https://css-tricks.com/all-about-floats/

* float is a CSS positioning property
* floated elements remain a part of the flow of the web page
* can be used for complete layouts in smaller instances
* the sister property of float is *clear* which, when placed on an element, allows it to remove itself from the flow of the other floated items and remain below them
    * has four values: *both, left, right and none*

# Don't overthink it grids
https://css-tricks.com/dont-overthink-it-grids/

* grids are great for laying out the main elements of pages

# CSS Floats Explained By Riding an Escalator
https://www.freecodecamp.org/news/css-floats-explained-by-riding-an-escalator-57fa55232333/

* so basically, not using float is like a jerk standing in the middle of the escalator, whereas using floats allows other images on the page to walk up the escalator faster because people (who are not jerks) are sticking to one side or the other

# Reference material: Scalable and Modular Architecture for CSS
http://smacss.com/