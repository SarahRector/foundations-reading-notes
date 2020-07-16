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