# Local Storage

## Introducing HTML5 Storage

* HTML5 Storage allows webpages to save named key/value pairs within the client web browser.
* This data is saved even after the browser is closed.
* The data is never transmitted to the remote web server, (unless otherwise specified) unlike cookies.
* It is supported on almost every browser.
* Data is stored on a named key (a string) which you will use to retrieve the data as well.
* We can store any JavaScript datatype (strings, booleans, integers, floats) using HTML5 storage.
* The data is stored as a string.
* If we are retrieving other data types we will need to use functions such as `parseInt()` or `parseFloat()` to coerce retrieved data into the expected JavaScript datatype.
* We can call `setItem()` with an existing name key to overwrite the previous value
* To erase a key and value we can use `removeItem()`
* To get the total number of values in the storage area, and to iterate through all of the keys by index in order to get the name of each key, we can use `key()`
* The `storageEvent` object has several useful properties including:
    - **key:** the named key that was added, removed, or modified
    - **oldValue:** any	the previous value (now overwritten), or null if a new item was added
    - **newValue:** any	the new value, or null if an item was removed
    - **url:** string	the page which called a method that triggered this change




