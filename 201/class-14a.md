# CSS Transforms, Transitions, and Animations

-------------------------------------------------

## CSS transform :

- **The transform property** applies a 2D or 3D transformation to an element. This property allows you to *example:* rotate, scale, move, skew, elements.


-  **Syntax :**

     transform: none|transform-functions|initial|inherit;



- **Values :**

Value | Description
---------- | -----------
none | Defines that there should be no transformation
matrix | Defines a 2D transformation, using a matrix of six values
translate(x,y) | Defines a 2D translation 
translate3d(x,y,z) | Defines a 3D translation 
translateX(x) | Defines a translation, using only the value for the X-axis
translateY(y) | Defines a translation, using only the value for the Y-axis
translateZ(z) | Defines a 3D scale transformation by giving a value for the Z-axis 
rotate(angle) | Defines a 2D rotation, the angle is specified in the parameter 
skew(x-angle,y-angle) | Defines a 2D skew transformation along the X- and the Y-axis
initial | Sets this property to its default value
inherit | Inherits this property from its parent element


------------------------------------------------


## CSS Transition 

- Allows you to change property values smoothly.

- To create transition you should specify the property and time of the effect.


- **Transition Properties :**

1. *transition-timing-function* : specifies the speed curve of the transition effect.

**Values**

Value | Description
--------- | -------------
ease | pecifies a transition effect with a slow start, then fast, then end slowly
linear | specifies a transition effect with the same speed from start to end
ease-in | specifies a transition effect with a slow start
ease-out | specifies a transition effect with a slow end
ease-in-out | specifies a transition effect with a slow start and end


2. *transition-delay* : specifies a delay (in seconds) for the transition effect.

3. *transition-duration* : Specifies how many seconds or milliseconds a transition effect takes to complete.

4. *transition-property* : Specifies the name of the CSS property the transition effect is for.


![animation](https://miro.medium.com/max/1400/1*spiB7DFGUs_-2HOo589Eug.png)