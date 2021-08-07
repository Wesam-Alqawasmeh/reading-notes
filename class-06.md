# JS Object Literals & The DOM


## Objects :

- Objects group together a set of variables and functions.

- In an object, variables and functions take on new names:

1. VARIABLES BECOME KNOWN AS PROPERTIES.

2. FUNCTIONS BECOME KNOWN AS METHODS.


![object](https://cdn.programiz.com/sites/tutorial2program/files/javascript-object-properties.png)




**Accessing an Object and Dot notation**

- Access the properties or methods using dot notation.

*Example*

    var example = Object.property;
    var I = Object.method;




## DOM :

**What is DOM:**

- The Document Object Model (DOM) is a programming interface for HTML and XML documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects. That way, programming languages can connect to the page.


- The HTML DOM model is constructed as a tree of Objects:


![dom](https://1.bp.blogspot.com/-BhSi2uyo_qM/WYrv62wLGJI/AAAAAAAABds/0oVq6Wgvx9A6aLrVbEE3hN7DOGVEs6-ZwCPcBGAYYCw/w400/12121212.gif)


![dom](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/08/Js-Dom-Tree.png)


**Finding HTML Elements**

- Finding HTML elements by id

- Finding HTML elements by tag name

- Finding HTML elements by class name

- Finding HTML elements by CSS selectors

- Finding HTML elements by HTML object collections



*example*

     const element = document.getElementById("id");

    let element = document.getElementsByTagName("T");

    const element = document.getElementsByClassName("class");
