# CHEATSHEET

## Tips

- When Horizontal padding is double the vertical, it usually looks good.

## Tools

Diffchecker.com

## BOX MODEL

### Block level boxes/elements occupy all the space that they can, from left to right, and they create line breaks after them.(display: block)

- elements are formatted visually as blocks
- elements are stacked vertically by default, one after another
- most of the HTML elements are block level elements: body, main, header, footer, section, nav, aside, div, h1-h6, p, ul, ol, li....
  - with CSS: (display: block)

### Inline boxes and elements occupy only space the size of their content(display: inline)

- Occupies only the space neccessary for its content
- causes no line-breaks
- box model applies in a different way: heights and witdth do not apply
- Paddings and margin are applied only horizontaly (even though in dev tools it shows as applied)

### Inline block boxes looks like an inline from the outside and behaveds like block-level on the inside(display: inline-block)

- occupies only content space
- causes no line-breaks
- box model applies as showed:
  - we can set heights and widths
  - we can use margins and paddings as with block-level

## Absolute positioning

### Normal flow:

- elements is "in flow"
- Elements are simply laid out according to their order in the HTML code

- Default positioning (position: relative;)

### Absolute positioning/Out of flow

- Element is removed from the normal flow: "out of flow"
- No impact on the surrouding elements, might even overlap them

- We use `top, bottom, left or right` to offset the element from its relatively positioned container

  - these `top, bottom, left or right` properties are definition of where element is positioned in relation to the viewport or !FIRST! relatively positioned(position: relative;) parent element.

- (position: absolute;)

## Pseudo-elements

- Pseudo elements are the elemnts that dont exists exists in HTMl but that we can still style
- use `::` to use Pseudo elements
- youcan also use "adjecent sibling element" selector by stating element + element and then pseudo element selector like `h3 + a::first-line {}`
- after will create pseudo element that will automatically selects the very first child
- any pseudo element is by default a inline element

## CSS Layouts

- what is the Layout?
  - Layout is the way text, images and other content is placed and arranged o a webpage
  - Layout gives the page visual structure, into which we place out content
  - **Building a layout**: arranging page elements into a visual structure, instead of simply having them placed one after another (normal flow)

### Page layout vs Component layout

- In a page layout, elements are laid out around the webpage
- in component layout, elements have their own layout inside the component, since the components are often composed out of multiple elements

### Float layouts

- The old way of building layouts of all sizes, using the `float` CSS property

### Flexbox layouts

- modern way of building one dimensional layouts
- it is basically row withou using floats
- perfect for component layouts

### CSS Grid

- modern way for laying out elements in 2 dimensional grid
- Perfect for page layouts and complex components
