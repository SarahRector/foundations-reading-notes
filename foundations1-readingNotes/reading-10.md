# Javascript & Jquery
## Chapter 10: Error handling and debugging

* knowing how the scripts are processed (what order) helps deal with errors because some scripts can't run without others running first
* errors throw *exceptions* 
* error objects help you figure out where the error is occurring 
    * **error** is generic
    * __syntax error__ means syntax hasn't been followed
    * **reference error** tried to reference a variable that is not declared or within scope
    * **type error** unexpected data type
    * **range error** numbers are not in acceptable range
    * **URI error** uses URI methods incorrectly
    * **eval error** eval function not used correctly
* can use other methods to write to the console to help with debugging
    * console.info can be used to hold info
    * console.warn can make warnings
    * console.error holds errors
* use breakpoints (debugger) to freeze the execution of code so you can see what is happening
    * can also make breakpoints conditional by right clicking on line and selecting "add conditional breakpoint"
* you can throw your own errors with ```throw new Error('message')```