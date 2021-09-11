# HTML Lists, Control Flow with JS, and the CSS Box Model

## HTML Book CH.(3,13)

### Lists

#### - HTML Unordered Lists
An unordered list is a collection of related items that have no special order or sequence. This list is created by using HTML <*ul*> tag. Each item in the list is marked with a bullet.

**Example**


    <*!DOCTYPE html*>
    <*html*>
      <*head*>
       <*title*>HTML Unordered List<*/title*>
      <*/head*>
      <*body*>
      <*ul*>
        <*li*>Name<*/li*>
        <*li*>Age<*/li*>
        <*li*>Major<*/li*>
      <*/ul*>
     <*/body*> 
    <*/html*>

#### - HTML Ordered Lists

If you are required to put your items in a numbered list instead of bulleted, then HTML ordered list will be used. This list is created by using <*ol*> tag. The numbering starts at one and is incremented by one for each successive ordered list element tagged with <*li*>

#### - Definition Lists
The definition list is created with
the <*dl*> element and usually
consists of a series of terms and
their definitions.
Inside the <*dl*> element you will
usually see pairs of <*dt*> and
<*dd*> elements.

### Boxes

**Box Dimensions**

- By default a box is sized just big
enough to hold its contents. To
set your own dimensions for a
box you can use the height and
width properties.
The most popular ways to
specify the size of a box are
to use pixels, percentages, or
ems. Traditionally, pixels have
been the most popular method
because they allow designers to
accurately control their size.

*Example*

      div.box {
      height: 300px;
      width: 300px;
      background-color: #bbbbaa;}



**Limiting Width**
- the
min-width property specifies
the smallest size a box can be
displayed at when the browser
window is narrow, and the
max-width property indicates
the maximum width a box can
stretch to when the browser
window is wide.

*Example*

    div.description {
    min-width: 450px;
    max-width: 650px;
    text-align: left;}


**Overflowing content**

- The overflow property tells the
browser what to do if the content
contained within a box is larger
than the box itself. It can have
one of two values:

1. hidden : This property simply hides any
extra content that does not fit in
the box.

2. scroll : This property adds a scrollbar to
the box so that users can scroll
to see the missing content. 


*Example*

    p.one {
    overflow: hidden;}
    p.two {
    overflow: scroll;}




**Border, Margin & Padding**

![Border img](https://sabe.io/classes/css/css-box-model-padding-border-margin/css-box-model.png)


- **Border Width** : The border-width property
is used to control the width
of a border. The value of this
property can either be given
in pixels or using one of the
following values:
thin
medium
thick
(You cannot use percentages
with this property.)

- **Border Style** : You can control the style of a
border using the border-style
property. This property can take
the following values:

1. solid : a single solid line.
2. dotted : a series of square dots.
3. dashed : a series of short lines.
4. double : two solid lines.
5. groove : appears to be carved
into the page.
6. ridge : appears to stick out from
the page.
7. inset : appears embedded into
the page.
8. outset : looks like it is coming
out of the screen.

- **More properties for boxes** 

|Name|link to read|
|-----|-----------|
|border color|[click](https://www.w3schools.com/cssref/pr_border-color.asp)|
|shorthand border|[click](https://www.w3schools.com/css/css_border_shorthand.asp)|
|centering content|[click](https://www.w3schools.com/css/css_align.asp)|
|display|[click](https://www.w3schools.com/css/css_display_visibility.asp)|
|border img|[click](https://www.w3schools.com/cssref/css3_pr_border-image.asp)|
|border shadows|[click](https://www.w3schools.com/cssref/css3_pr_box-shadow.asp)|



## JS Book Ch.(4)

**Switch statement**
- A switch statement is a type of selection control mechanism used to allow the value of a variable or expression to change the control flow of program execution via search and map.Switch statements function somewhat similarly to the *if* statement used in programming languages.

- switch statement starts with a
variable called the switch value.
Each case indicates a possible
value for this variable and the
code that should run if the
variable matches that value.


*syntax*

    switch(expression) {
      case x:
       // code block
       break;
       case y:
        // code block
       break;
       default:
       // code block
     }

![switch statement](https://beginnersbook.com/wp-content/uploads/2017/08/switch_case_flow_diagram.jpg)



**loops**

- For : loops through a block of code a number of times.

*syntax*

    for (statement 1; statement 2; statement 3) {
      // code block to be executed
    }


- While : loops through a block of code while a specified condition is true.

*syntax*

    while (condition) {
      // code block to be executed
    }


- Do while :  also loops through a block of code while a specified condition is true.

*syntax*
    do {
      // code block to be executed
    } 
    while (condition);

![loop counters](https://www.w3resource.com/w3r_images/c-for-statement.png)



