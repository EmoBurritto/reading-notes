# Readings: CSS Layout

## Learn CSS - Flexbox

sidebar tricky in responsive design

txt can become squished and unreadable

flexbox is for one dimensional content

best for a lot of content of different sizes and variety

flex box does not have rigid dimensions

provides flexible boundaries

can display row or column

respect content size

single line by default

vs DOV, content can be moved around in order

space is not according to parent element

using box alignment properties, space can be distrubeted; flex lines wrapped

display: flex; for flexbox will give block-level box with flex item children  

flex means display items in a row; do not wrap; do not grow to fill container; line up at start of container

flex direction is row by default

row: items in a row

row-reverse: items in a row at end of flex container

column: items displayed in acolumn

column-reverse: items displayed in a column at end of flex container

flex-wrap default is no wrap

## Questions

1. Flexbox is designed for one-dimensional content. Explain what this means.

Best for a lot of content with different sizes by providing non rigid enviornment for content to rendly freely for user friendliness

2. Explain the difference between the main axis and cross axis.

main axis: horizontal; row; set by felx-direction property

cross axis:  vertical; column; oppposite of main axis

3. How can using certain properties of flexbox negatively impact accessibility?

There are defaults that can negatively affect flow; also know when to use reverse

## CSS Layout - Flexbox

floats and  positioning old way of doing things

flex gives:

vertically centering a block of content inside its parent

making children elements all equal

making all columns same size

for display, use parent for property to affect children

inline-flex: to make children elements into a flex items

cross axis: running perpendicular to main axis; direction flex items are displayed

wrap: prevent children element be displayed outside container

flex-flow: short hand for direction and wrap in that order

flex: number; gives spaces for content in flex line 

flex short hand affect grow, shrink and basis 

## Questions

1. What are some advantages of using flexbox over float?

vertically centering a block of content inside its parent

making children elements all equal

making all columns same size

flex-flow: short hand for direction and wrap in that order

2. How does this topic connect with your long term goals?

Correctly display site using CSS following matrix given by a potential customer.

## Things to Know

- need to know more developer podcast, LOVE IT
- need explanation on flex-direction
- when to use reverse
