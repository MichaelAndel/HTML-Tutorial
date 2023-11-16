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