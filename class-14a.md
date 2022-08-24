# Class 14a - CSS Transforms, Transitions, and Animations

---

## CSS Transforms

---

### 2D Stuff


- 2D Rotate: The rotate value provides the ability to rotate an element from 0 to 360 degrees.

Example:

    < figure class="box-1"> Box 1 </figure>
    < figure class="box-2"> Box 2 </figure>

        .box-1 {
          transform: rotate(20deg);
        }
        .box-2 {
          transform: rotate(-55deg);
        }

- 2D Scale: allows you to change the appeared size of an element.

Example:

    <figure class="box-1"> Box 1 </figure>
    <figure class="box-2"> Box 2 </figure>

    .box-1 {
      transform: scale(.75);
    }
    .box-2 {
      transform: scale(1.25);
    }

- 2D Translate: The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document.

Example:

    <figure class="box-1">Box 1</figure>
    <figure class="box-2">Box 2</figure>
    <figure class="box-3">Box 3</figure>

    .box-1 {
        transform: translateX(-10px);
    }
    .box-2 {
        transform: translateY(25%);
    }
    .box-3 {
        transform: translate(-10px, 25%);
    }

- 2D Skew: used to distort elements on the horizontal axis, vertical axis, or both.

Example:

    <figure class="box-1">Box 1</figure>
    <figure class="box-2">Box 2</figure>
    <figure class="box-3">Box 3</figure>

    .box-1 {
        transform: skewX(5deg);
    }
    .box-2 {
        transform: skewY(-20deg);
    }
    .box-3 {
        transform: skew(5deg, -20deg);
    }

## 3D Stuff

- 3D Rotate: with three-dimensional transforms we can rotate an element around any axes. To do so, we use three new transform values, including rotateX, rotateY, and rotateZ.

Example:

    <figure class="box-1">Box 1</figure>
    <figure class="box-2">Box 2</figure>
    <figure class="box-3">Box 3</figure>

    .box-1 {
        transform: perspective(200px) rotateX(45deg);
    }
    .box-2 {
        transform: perspective(200px) rotateY(45deg);
    }
    .box-3 {
        transform: perspective(200px) rotateZ(45deg);
    }

- 3D Scale: By using the scaleZ three-dimensional transform elements may be scaled on the z axis. the rotateX value is added in order to see the behavior of the scaleZ value.

Example:

    <figure class="box-1">Box 1</figure>
    <figure class="box-2">Box 2</figure>

    .box-1 {
    transform: perspective(200px) scaleZ(1.75) rotateX(45deg);
    }
    .box-2 {
    transform: perspective(200px) scaleZ(.25) rotateX(45deg);
    }

- 3D Translate: Elements may also be translated on the z axis using the translateZ value. A negative value here will push an element further away on the z axis, resulting in a smaller element.

Example:

    <figure class="box-1">Box 1</figure>
    <figure class="box-2">Box 2</figure>

    .box-1 {
    transform: perspective(200px) translateZ(-50px);
    }
    .box-2 {
    transform: perspective(200px) translateZ(50px);
    }

- 3D Skew: Skew is the one two-dimensional transform that cannot be transformed on a three-dimensional scale. Elements may be skewed on the x and y axis, then transformed three-dimensionally as wished, but they cannot be skewed on the z axis.

---

[CSS Transformations Website](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

---

## CSS Transitions and Animations

### Transitions

    For a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the: 
    
    :hover, :focus, :active, and :target pseudo-classes.

There are four transition related properties in total:  

    transition-property, transition-duration,transition-timing-function, and transition-delay. 

    Not all of these are required to build a transition, with the first three are the most popular.

Example: 

    .box {
        background: #2db34a;
        transition-property: background;
        transition-duration: 1s;
        transition-timing-function: linear;
    }
    .box:hover {
        background: #ff7b29;
    }

- Transitional Property: the transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties.

Transitional Properties:

    background-color    background-position
    border-color        border-width
    border-spacing      bottom              
    clip                colorcrop
    font-size           font-weight
    height              left
    letter-spacing      line-height 
    margin              max-height
    max-width           min-height  
    min-width           opacity 
    outline-color       outline-offset
    outline-width       padding
    right               text-indent
    text-shadow         top
    vertical-align      visibility
    width               word-spacing

Transition Duration

Transition Timing

Transition Delay

### Shorthand Transitions

    There is a shorthand property, "transition", capable of supporting all of these different properties and values. Using the transition value alone, you can set every transition value in the order of transition-property, transition-duration, transition-timing-function, and lastly transition-delay. Do not use commas with these values unless you are identifying numerous transitions.

Example: 

    .box {
    background: #2db34a;
    border-radius: 6px;
    transition: background .2s linear, border-radius 1s ease-in 1s;
    }
    .box:hover {
    color: #ff7b29;
    border-radius: 50%;
    }

Transitional Button

    <button> Awesome Button </button>

    button {
    border: 0;
    background: #0087cc;
    border-radius: 4px;
    box-shadow: 0 5px 0 #006599;
    color: #fff;
    cursor: pointer;
    font: inherit;
    margin: 0;
    outline: 0;
    padding: 12px 20px;
    transition: all .1s linear;
    }
    button:active {
    box-shadow: 0 2px 0 #006599;
    transform: translateY(3px);
    }

### Animations

Animation Keyframes

    To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

Example

    @keyframes slide {
    0% {
        left: 0;
        top: 0;
    }
    50% {
        left: 244px;
        top: 100px;
    }
    100% {
        left: 488px;
        top: 0;
    }
    }

### Customizing Animations

---

[CSS Transitions and Animations Website](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)

---

## 8 simple transitions

[CSS Transformations Website](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

## Things I want to know more about

- I need to practice CSS more..

[Previous Page](https://tomgtaylor.github.io/reading-notes2/class-13)    ||    [Next Page](https://tomgtaylor.github.io/reading-notes2/class-14b) <br>

---
[HOME](https://tomgtaylor.github.io/reading-notes2) <br>
