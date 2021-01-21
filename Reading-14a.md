# Reading 14a

***CSS Transforms***
- CSS allows you to change elements on a 2d or a 3d plane
- you can combine different transformative elements as you need 
- you can also change how elements are perceived. 
  - this can be done by changing the perspective depth value using CSS. For example: transform: perspective(75px) rotateX(40deg)
- if you rotate a 3d element to view its backside, you can customize that part of the element or hide it using backface-visibility

***CSS transitions and Animations***
- Using pseudo-classes we can use four different transition properties to build a transforming element. 
  - the pseudo classes are: :hover, :focus, :active, and :target and the transition properties are: transition-property, transition-duration, transition-timing-function, and transition-delay
- many of the same properties that we use in normal CSS styling are available for use here. Including items like height, width, background-color etc. 
- to start an animation we should us an @keyframe/s rule. 

***CSS3 Transitions***
- Using the :hover pseudo class we can use many cool transitions such as:
  - .fade which will fade the background
  - .color which will change the background color
  - .grow or .shrink which will either grow or shrink the object
  - use .rotate to rotate a given object a certain direction
  - .circle causes it to change shape to a circle 
  - .threed gives it a small 3d shadow. Or big. You pick.
  - .swing will move the object side to side 
  . and finally box shadow causes it to appear to shrink and gives it an inner border
