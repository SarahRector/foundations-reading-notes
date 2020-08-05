# HTML & CSS
## Chapter 7: Forms (p.144-175)

* Lots of different options for collecting info from users (inputs, raido buttons, checkboxes, drop downs, etc)
* how a form works:
    * user enters info, clicks a button, name of form conrtol is sent to the server along with user inputs, server processes info, then surver creates a new page to send back to the browser
* uses ```<form>``` element that contains an *action* (the url for where on the server the info is going), sometimes a *method* and and *id*
* text input uses the ```<input>``` element which uses ```type="text" or "number"```, *name* and can also use *min/max length*
    * can create a password input using ```<input type="password">```
    * ```<textarea>``` creates a multi-line text input using ```cols="20" and rows="4"``` or however big you want it
* ```<input type="radio">``` creates radio buttons and uses *name*, *value* (which is the value sent to the server if the button is checked), and *checked* (which indicates that this button should be checked when the page loads)
* ```<input type="checkbox">```creates checkboxes that can be used to indicate more than one thing and use *name, value and checked* just like radio buttons
* drop down lists can be created using ```<select>``` and take a *name*
    * options on the drop down menu are created using ```<option>``` and takes a *value* which is the option that appears on the list and is also what is sent to the server
    * to allow users to select more than one thing on the drop down, use ```multiple="multiple"```
* if you want people to upload a file use ```<input type="file">```
* for a submit button use ```<input type ="submit">``` the *value* will be the text that appears on the button
    * to make an image be the submit button use ```<input type="image">```
* each form control should have a ```<label>``` element with it
    * can either wrap the form control or be seperate from it and use the *for* attribute: ```<label for="cat input">Input your cat here!</label>```
* to group form elements you can use ```<fieldset>``` which groups the elements together with a line around the edge and then ```<legend>``` which comes directly after the fieldset tag and contains a caption which helps id the purpose of that group of form controls
* can also specify type of info to be input like *date, email, url*
* ```type="search"```makes a specific search input and *placeholder* allows you to have text in that search area until someone types something in it


## Chapter 14: Lists, Tables & Forms (p.330-357)

* in CSS, the ```list-style-type``` property allows you to control the shape of the bullet point in an unordered list
    * can use *none, disc, circle, square*
* in an ordered list, it can be used to specify as well
    * *decimal (number), decimal-leading-zero (number with a zero in front), lower-alpha (lower case letters), upper-alpha, lower-roman and upper-roman*
* can also make images into bullets with ```list-style-image: url(the url of the image here)```
* ```list-style-position``` lets you specify if the marker is contained inside or outside of the box containing the list
* there are lots of different table properties
* buttons, text inputs, fieldsets, ledgends can all be styled


# Javascript & Jquery
## Chapter 6: Events (p.243-292)

* several outdated ways to do handle events, best practice is using event listeners with ```addEventListener()```
    * older versions of internet explorer are not always great with event listeners
* the flow of your code matters with event listeners because if things are nested within it, they have an order to the way they will happen
* *load* is an event that is used to trigger scripts
* *focus and blur* are triggered when dom elements come into or out of focus
* *click* is triggered when something is clicked
* event listeners can also be used to show position of the mouse when something was clicked, or record which key was pressed