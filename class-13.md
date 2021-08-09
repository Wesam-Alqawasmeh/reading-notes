# Local Storage 

------------------------------------------

## HTML Web Storage :

- web applications can store data locally within the user's browser.


- Before HTML5, application data had to be stored in cookies, included in every server request.

- the storage limit is far larger (at least 5MB) and information is never transferred to the server.

- Web storage is per origin (per domain and protocol). All pages, from one origin, can store and access the same data.


## HTML web storage objects :

1. **window.localStorage:**  stores data with no expiration date.

2. **window.sessionStorage:** stores data for one session.


## Using HTML5 Storage :

- *HTML5 Storage* is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats.

- The data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like **parseInt() or parseFloat()** to coerce your retrieved data into the expected JavaScript datatype.


## Traking changes to the HTML5 Area :


- If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever **setItem(), removeItem(), or clear()** is called and actually changes something.



### Storage event project :

PROPERTY | TYPE | 	DESCRIPTION
-------- | ------- | ------------
key | string | the named key that was added, removed, or modified
oldValue | any | the previous value (now overwritten), or null if a new item was added
newValue | any | the new value, or null if an item was removed 
url | string | the page which called a method that triggered this change


![localstorage](https://scriptverse.academy/img/tutorials/html5-localstorage.png)

