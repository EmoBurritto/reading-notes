# CSS 

CSS3 = new ways to position and alter elements

transform property comes in two different settings, two-dimensional and three-dimensional

div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);

transform: value specifies the transform type followed by a specific amount inside parentheses

prefixes first then just transform to accomadate different browsers 

two-dimensional: x and y axis 

three-dimensional: x, y and z axis (depth)

default rotate 50%, 50%, rotate counter clockwise 

scale: change its size, deault value 1 

translate: like relative positoning, squish other elements

skew: change x, y axis position 

to combine use comma only use two not multiple 

perspective: vanishing point needed for three dimensional transform 

## CSS Transforms

(reference: https://learn.shayhowe.com/advanced-html-css/css-transforms/)

## Questions 

1. What does a CSS transform allow the developer to do to an element?

transform: two-dimensional and three-dimensional property to an element 

2. Provide an example of a transform and how you could see that being used on a website.

.box-2 {
  transform: rotate(-55deg);

  rotate and image -55  degrees so its slanted for effect on a site 
          

## CSS Transitions & Animations

use  :hover, :focus, :active, and :target pseudo-classes for transitions

4 main transition properties: 

- transition-property
- transition-duration
- transition-timing-function
- transition-delay

Other Transitional Properties: 

- background-color
- background-position
- border-color
- border-width
- border-spacing
- bottom
- clip
- color
- crop
- font-size
- font-weight
- height
- left
- letter-spacing
- line-height
- margin
- max-height
- max-width
- min-height
- min-width
- opacity
- outline-color
- outline-offset
- outline-width
- padding
- right
- text-indent
- text-shadow
- top
- vertical-align
- visibility
- width
- word-spacing

Keyframes:

- @-moz-keyframes
- @-o-keyframes
- @-webkit-keyframes

(reference: https://learn.shayhowe.com/advanced-html-css/transitions-animations/)

## Questions 

1. What does a CSS transition allow the developer to do to an element?

allows for user friendly transition between affected properties 

2. How does a CSS animation differ from a CSS transition?

multiple state of transitions for desired element 

## 8 simple CSS3 transitions that will wow your users

Fade in: 
.fade
{
        opacity:0.5;
}
.fade:hover
{
        opacity:1;
}

Change Color: 

.color:hover
{
        background:#53a7ea;
}

Grow and Shrink: 

.grow:hover
{
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
}

.shrink:hover
{
        -webkit-transform: scale(0.8);
        -ms-transform: scale(0.8);
        transform: scale(0.8);
}

Rotate Elements:

.rotate:hover
{
        -webkit-transform: rotateZ(-30deg);
        -ms-transform: rotateZ(-30deg);
        transform: rotateZ(-30deg);
}

Square to Circle:

.circle:hover
{
        border-radius:50%;
}

3D shadow:

.threed:hover
{
        box-shadow:
                1px 1px #53a7ea,
                2px 2px #53a7ea,
                3px 3px #53a7ea;
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
}

Swing:
@-webkit-keyframes swing
{
    15%
    {
        -webkit-transform: translateX(5px);
        transform: translateX(5px);
    }
    30%
    {
        -webkit-transform: translateX(-5px);
       transform: translateX(-5px);
    } 
    50%
    {
        -webkit-transform: translateX(3px);
        transform: translateX(3px);
    }
    65%
    {
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
    }
    80%
    {
        -webkit-transform: translateX(2px);
        transform: translateX(2px);
    }
    100%
    {
        -webkit-transform: translateX(0);
        transform: translateX(0);
    }
}
@keyframes swing
{
    15%
    {
        -webkit-transform: translateX(5px);
        transform: translateX(5px);
    }
    30%
    {
        -webkit-transform: translateX(-5px);
        transform: translateX(-5px);
    }
    50%
    {
        -webkit-transform: translateX(3px);
        transform: translateX(3px);
    }
    65%
    {
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
    }
    80%
    {
        -webkit-transform: translateX(2px);
        transform: translateX(2px);
    }
    100%
    {
        -webkit-transform: translateX(0);
        transform: translateX(0);
    }
}
.swing:hover
{
        -webkit-animation: swing 1s ease;
        animation: swing 1s ease;
        -webkit-animation-iteration-count: 1;
        animation-iteration-count: 1;
}

Inset Border:

.border:hover
{
        box-shadow: inset 0 0 0 25px #53a7ea;
}
(reference: https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users/)

## Questions 

1. What are some benefits to using CSS transitions on websites?

Allows for user friendliness and attractivness to use site; also very common requests from clients 

2. How this topic fit in with your long-term goals?

This will be awesome if I were to contract and to satisfy client requirements. Even in unemployment, I can beef up my projects to display what I can do to future employers. 

## Things I want to know more about 
- animations 