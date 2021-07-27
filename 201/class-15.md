## CSS Transforms, Transitions, and Animations

### **Transforms**

- With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.

- The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

#### Transform Syntax
The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

    div {
       -webkit-transform: scale(1.5);
       -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
        transform: scale(1.5);
    }

### 2D Transforms
Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth.

#### 2D Rotate
The rotate() method rotates an element clockwise or counter-clockwise according to a given degree.

#### 2D translate
The translate() method moves an element from its current position (according to the parameters given for the X-axis and the Y-axis).

#### 2D scale
The scale() method increases or decreases the size of an element (according to the parameters given for the width and height).

#### 2D skew
The skewX() method skews an element along the X-axis by the given angle.

![Image](https://miro.medium.com/max/1400/1*_NVMTnvHTM9teQxrVRlDeg.png)

---

### 3D Transforms
Working with two-dimensional transforms we are able to alter elements on the horizontal and vertical axes, however there is another axis along which we can transform elements. Using three-dimensional transforms we can change elements on the z axis, giving us control of depth as well as length and width.

### CSS 3D Transform Methods

Function | Description | 
----|-----
matrix3d |Defines a 3D transformation, using a 4x4 matrix of 16 values| 
translate3d(x,y,z) |Defines a 3D translation|
translateX(x) |Defines a 3D translation, using only the value for the X-axis| 
translateY(y) |Defines a 3D translation, using only the value for the Y-axis|
translateZ(z) |Defines a 3D translation, using only the value for the Z-axis| 
scale3d(x,y,z) |Defines a 3D scale transformation|
scaleX(x) |Defines a 3D scale transformation by giving a value for the X-axis|
scaleY(y) |Defines a 3D scale transformation by giving a value for the Y-axis| 
scaleZ(z) |	Defines a 3D scale transformation by giving a value for the Z-axis|
rotate3d(x,y,z,angle) |Defines a 3D rotation| 
rotateX(angle) |Defines a 3D rotation along the X-axis|
rotateY(angle) |Defines a 3D rotation along the Y-axis| 
rotateZ(angle) |Defines a 3D rotation along the Z-axis|

---

## Transitions & Animations

- One evolution with CSS3 was the ability to write behaviors for transitions and animations. Front end developers have been asking for the ability to design these interactions within HTML and CSS, without the use of JavaScript or Flash

- With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.

- Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.

### Transitions
 for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the **:hover**, **:focus**, **:active**, and **:target** pseudo-classes.

There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.

### How to Use CSS Transitions?
- To create a transition effect, you must specify two things:

1-the CSS property you want to add an effect to  
2-the duration of the effect  
**Note:** If the duration part is not specified, the transition will have no effect, because the default value is 0.

    div {
    width: 100px;
    height: 100px;
    background: red;
    transition: width 2s;
    }

#### Specify the Speed Curve of the Transition
The transition-timing-function property specifies the speed curve of the transition effect.

- The transition-timing-function property can have the following values:

**ease** - specifies a transition effect with a slow start, then fast, then end slowly (this is default)  
**linear** - specifies a transition effect with the same speed from start to end  
**ease-in** - specifies a transition effect with a slow start  
**ease-out** - specifies a transition effect with a slow end  
**ease-in-out** - specifies a transition effect with a slow start and end  
**cubic-bezier(n,n,n,n)** - lets you define your own values in a cubic-bezier function

#### Delay the Transition Effect
The transition-delay property specifies a delay (in seconds) for the transition effect.

    div {
    transition-delay: 1s;
    }

### CSS Transition Properties
- The following table lists all the CSS transition properties:

Property | Description | 
----|-----
transition |A shorthand property for setting the four transition properties into a single property|
transition-delay |Specifies a delay (in seconds) for the transition effect|
transition-duration |Specifies how many seconds or milliseconds a transition effect takes to complete|
transition-property |Specifies the name of the CSS property the transition effect is for|
transition-timing-function |Specifies the speed curve of the transition effect|

----

## Animations

- Transitions do a great job of building out visual interactions from one state to another, and are perfect for these kinds of single state changes. However, when more control is required, transitions need to have multiple states. In return, this is where animations pick up where transitions leave off.

#### Animations Keyframes
- To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

### Animation Name
Once the keyframes for an animation have been declared they need to be assigned to an element. To do so, the animation-name property is used with the animation name, identified from the @keyframes rule, as the property value. The animation-name declaration is applied to the element in which the animation is to be applied to.

    .stage:hover .ball {
    animation-name: slide;
    }

### Animation Duration, Timing Function, & Delay

The animation-delay property specifies a delay for the start of an animation.

    .stage:hover .ball {
    animation-duration: 2s;
    }

### Animation Iteration

The animation-iteration-count property specifies the number of times an animation should run.

      div {
      animation-name: example;
      animation-duration: 4s;
      animation-iteration-count: 3;
      }

### Animation Direction

- The animation-direction property specifies whether an animation should be played forwards, backwards or in alternate cycles.

- The animation-direction property can have the following values:

**normal** - The animation is played as normal (forwards). This is default  
**reverse** - The animation is played in reverse direction (backwards)  
**alternate** - The animation is played forwards first, then backwards  
**alternate-reverse** - The animation is played backwards first, then forwards

     div {
     animation-direction: reverse;
     }

### Specify the fill-mode For an Animation
- CSS animations do not affect an element before the first keyframe is played or after the last keyframe is played. The animation-fill-mode property can override this behavior.

- The animation-fill-mode property specifies a style for the target element when the animation is not playing (before it starts, after it ends, or both).

- The animation-fill-mode property can have the following values:

**none** - Default value. Animation will not apply any styles to the element before or after it is executing  
**forwards** - The element will retain the style values that is set by the last keyframe (depends on animation-direction and animation-iteration-count)  
**backwards** - The element will get the style values that is set by the first keyframe (depends on animation-direction), and retain this during the animation-delay period  
**both** - The animation will follow the rules for both forwards and backwards, extending the animation properties in both directions     

![Image](https://i.stack.imgur.com/h1Mt1.gif)