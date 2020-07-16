# Article: "The Past, Present, and Future of Local Storage for Web Applications"

* cookies may not be great (though delicious) because:
    * they slow things down
    * they send unencrypted data
    * they're limited to a pretty small size
* preferred would be something with:
    * lots of space
    * on the client
    * stays beyond refreshing the page
    * isn't transmitted to the server

* History of local storage hacks before HTML5
    * Internet Explorer had userData
        * allows web pages to store up to 64KB of data
    * Adobe introduces "Flash cookies" - a local shared object
    * 2007 Google made "Gears" which was a browser plug-in
    * all were either specific to a particular browser or needed a plug-in

* HTML5 Storage
    * Web Storage - aka local storage
        * a way for web pages to store named key/value pairs locally within the web browser
            * it persists after you navigate away from the website
            * available even when third-party browser plugins are not

* Using HTML5 Storage
    * based on named key/value pairs
    * keys are always stored as a string
    * setItem() sets the key in local storage
    * getItem() gets the key from local storage

* Tracking Changes to the HTML5 Storage Area
    * storage event is supported everywhere localStorage object is supported

* Limitations in Current Browsers
    * each origin gets 5 megabytes of storage by default

* HTML Storage in Action
    * like in a game, you can close the browser window and not lose your progress with local Storage
    * does this by iterating through the pieces and saving the row and column number of each piece (for example), and then calls a ```resumeGame()```function

* Beyone Named Key-Values Pairs: Competing Visions
    * SQL - like backend database programming except you're doing it from JavaScript