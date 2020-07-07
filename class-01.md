# foundations-reading-notes

## HTML&CSS 
# Introduction
    * how book is structured
    * how people access the web
        * browsers
        * web servers
        * devices
        * scteen readers
    * how websites are created
        * everything has HTML and CSS but there are other platforms used as well

# Structure
    * HTML describes the structure of the page using elements (also called tags)
        * most elements have an opening and closing tag that tell you something about what is between the opening and closing tag

    * Attributes are on the opening tag of the element and are made up of two parts: a name and a value

    * Types of tags
        * body: is everything shown in main browser window
        * head: has info about the page sometimes contains a title
        * title: what is shown in the top of the browser (on the tab)

# Extra Markup
    * Doctypes
        * tells the browser which version of HTML the page is using

    * Comments
        * comments are added to code because it helps explain why something is a certain way or what it was supposed to do. It makes it easier to understand.

        * can also be used to "comment out" blocks of code temporarially

    * Id Attrubute
        * uniquely identifies that element on the page

    * Class Attribute
        * used to identify groups of elements on the page

    * Block vs Inline Elements
        * block elements always start on a new line
        * inline elements continue on the same line as their neighboring elements

    * Div Elements
        * group text and elements together in a block
        * good for holding sections of the page

    * Span Elements
        * group text and elements inline
        * can also use to style a portion of text differently in CSS

    * IFrames
        * tiny window cut into page that displays another page
        * commonly used to embed google maps into a page

    * Meta Element
        * lives in the head
        * not visible to users but tells search engines about your page, cometimes has a description, author info, etc

    * Escape Charachters
        * certain characters that are used in HTML require other syntax for the character to actually appear on the page. For example copyright symbol must be written as &copy

# HTML5 Layout

    * sections of the page used to be grouped into all Div elements

    * now, new elements (header, nav, article, etc) help with semantic HTML and easier understanding of code

        * types of new elements
            * headers and footers: top and bottom sections of whole page or/and can be assigned to individual sections on a page
            * nav: primary site navigation or links
            * article: anything that could stand alone
            * aside: if inside an article, contains info related to the article but not essential to it's meaning (like a pullquote). If outside of an article, it contains content related to the entire page
            * section: usually has it's own heading, groups content together. Should not be used as a wrapper for the entire page
            * hgroup: groups headings together
            * figure and figcaption: contains content refrenced in main flow of an article (including images). figcaption is the caption for whatever is in the figure

# Process & Design
    
    * When building a site, think about who it's supposed to be for
        * individuals, companies, etc

    * Why are they using your site and what are they trying to get out of it?

    * What information will they want and how often will they want it?

    * Site maps
        * are a diagram of how the different pages on your site will be layed out or grouped together
            * looks like a family tree
            * helps organize the flow of the site

    * Wireframes
        * sketches that show the design of the site at a very basic level
            * what information goes where and how much space it takes up


## Javascript & Jquery

# Introduction

    * Javascript makes webpages more interactive by allowing users to:
        * access content
        * modify content
        * set up rules for the browser to follow
        * change based on events that occur (buttons clicked, input, time has passed, etc)

# The ABCs of Programming

    * Scripts
        * scripts are instructions that a computer follows to do something
        * to write a script break it down into several steps
            * what's the goal
            * make a flowchart to show the individual steps
            * write the code to accomplish each step

    * How do computers fit in with the real world?
        * they create models of the world using data such as objects, properties, events and methods

    * The Document Object
        * represents an HTML pace and allows you to change the content seen on a page and how users interact with it
