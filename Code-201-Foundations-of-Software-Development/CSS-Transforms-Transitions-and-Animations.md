# CSS Transforms  

* Transforms are a new way to position and alter elements.
    - comes in two different settings
1. Two-dimensional 
2. Three-dimensional

## Transform Syntax
* The syntax for the transform property includes the transform property and then the value
* The value consists of the transform type followed by a specific amount inside parentheses

Here's an example:
```
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}
```
## Two-Dimensional Transforms
* These transforms work on horizontal and vertical axes (x and y).
* Some examples of 2D values include:
    - 2D Rotate
    - 2D Scale
    - 2D Translate
    - 2D Skew
    - 2D Cube
    - 2D Perspective

## Three-Dimensional Transforms
* These transforms work on x, y, and z axes.
* Define length, width, and depth, of an element.
* Some examples of 3D values include:
    - 3D Rotate
    - 3D Scale
    - 3D Translate
    - 3D Skew
    - 3D Transform
    - 3D Backface Visibility
    - 3D Cube

# CSS Transitions & Animations 

## Transitions
* CSS3 Transitions alter the appearance and behavior of an element depending on a state change that occurs such as 
    - `:hover`
    - `:focus`
    - `:active`
    - `:target`
* There are four transition related properties:

1  **transition-property:** defines what properties will be altered
2. **transition-duration:** specifies how long a transition takes place is
3. **transition-timing-function:** used to set the speed in which a transition will move
4. **transition-delay:** sets a time value in seconds or milliseconds, that determines how long a transition should be stalled before executing

## Animations
* Animations allow us to set multiple points at which an element should change, where as transitions are for single state changes.
* We can use the `@keyframes` element to specify the animation name, breakpoints, and properties to be animated.
* Keyframe breakpoints are written with percentages, starting at 0% and go to 100%.
* After naming the animation we can add a duration, timing function, and delay.
* The duration is set using `animation-duration:` and it's value is written in seconds or milliseconds.
* `animation-timing-function` declares a timing function.
* `animation-duration:` declares the delay.
* Some animation properties we can use to customize an elements behavior include:
    - **animation-iteration-count:** allows us to make an animation repeat as many times as we specify or we can use infinite to make it repeat indefinitely. 
    - **animation-direction:** includes the direction an animation completes. we can use the following values: normal, reverse, alternate, and alternate-reverse.
    - **animation-play-state:** lets an animation be played or paused using the running and pause keywords.
    - **animation-fill-mode:** determines how an element will be styled either before, after, or before and after we run the animation using the values: none, forwards, backwards, and both.
    