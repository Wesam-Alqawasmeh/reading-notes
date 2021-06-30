# JS

## what is Javascript?
**JavaScript** (JS) is a lightweight, interpreted, or just-in-time compiled programming language with first-class functions. While it is most well-known as the scripting language for Web pages, many non-browser environments also use it, such as Node.js, Apache CouchDB and Adobe Acrobat. JavaScript is a prototype-based, multi-paradigm, single-threaded, dynamic language, supporting object-oriented, imperative, and declarative (e.g. functional programming) styles.


### Input & output in JS
*JavaScript* has a few window object methods that you can use to interact with your users. The prompt() method lets you open a client-side window and take input from a user. For instance, maybe you want the user to enter a first and last name. Normally, you can use an HTML form for user input, but you might need to get the information before sending the form back to your server for processing. You can use the window.prompt() method for small amounts of information. It's not meant for large blocks of text, but it's useful when you need information before the user continues to another page.

The following code is an example of the window.prompt method. 

var customerName = prompt("Please enter your name", "<name goes here>");

if (customerName!= null) {

    document.getElementById("welcome").innerHTML =

    "Hello " + customerName + "! How are you today?";

}

The first line of code uses the prompt method. Notice that we don't need the "window" object since JavaScript inherits the main DOM methods and understands that this is an internal method. The first parameter in the prompt is what you want to show the user. In this example, we want the user to enter a name, so the prompt displays "Please enter your name." The second parameter is the default text. This default text helps the user understand where to type the name, but if he clicks "OK" without entering a name, the "<name goes here>" text will be used for the username. You can create checks in your JavaScript code that detects when the user doesn't enter a name and just clicks OK, but this code assumes any text entered is the user's name.