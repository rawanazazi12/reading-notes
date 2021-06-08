# What I've Learned at the 14th/a lecture of 201 code

## Transforms

1. With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.

2. The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

3. **Transform Syntax**      
   The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

4. **2D Transforms**     

    - Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. 
    - Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes.
    - Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth.

5. **Combining Transforms**
    - It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time for example.
    - In this event multiple transforms can be combined together. 
    - To combine transforms, list the transform values within the transform property one after the other without the use of commas.

6. **Transform Origin**     
   The transform-origin property can accept one or two values. When only one value is specified, that value is used for both the horizontal and vertical axes. If two values are specified, the first is used for the horizontal axis and the second is used for the vertical axis.

## Transitions & Animations

### Transitions

1. With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.

2. There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.

3. **Transition Duration**
   - The duration in which a transition takes place is set using the transition-duration property. 
   - The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). 
   - These timing values may also come in fractional measurements, .2s for example.

4. **Transition Timing**    
  The transition-timing-function property is used to set the speed in which a transition will move. Knowing the duration from the transition-duration property a transition can have multiple speeds within a single duration.

5. **Transition Delay**     
  You can set a delay with the transition-delay property. The delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing. 

### Animations          

1. To set multiple points at which an element should undergo a transition, use the `@keyframes` rule. The `@keyframes` rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

2. **Animation Name**        
  Once the keyframes for an animation have been declared they need to be assigned to an element. To do so, the animation-name property is used with the animation name, identified from the @keyframes rule, as the property value.
 
3. **Animation Duration, Timing Function, & Delay**           
  Once you have declared the animation-name property on an element, animations behave similarly to transitions. They include a duration, timing function, and delay if desired. To start, animations need a duration declared using the animation-duration property. As with transitions, the duration may be set in seconds or milliseconds.


#### RESOURSES

- [CSS Transforms](https://learn.shayhowe.com/advanced-html-css/css-transforms/)
- [CSS Transitions & Animations](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)


