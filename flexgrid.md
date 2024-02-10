### General

#### normal flow of document
- elements are positioned on a page according to
  - the order in which they are written in the HTML
  - and whether their **behavior is inline or block**
    - one below the other for block-level elements
    - one next to the other for inline or inline-block level elements.
  - margins and padding used to control the space between the elements
- `position:` , `display:`, `float:` used to create layout before flex //TODO: example code.

  ### Flexbox
  - Flexbox is
    - a method to arrange elements **in one direction**
    - horizontally or vertically
    -  and control their dimensions, alignments, order of appearance and more.
  - need at least two elements
    - **a parent element called flex container**
    - and **at least one** child element called **flex item**.
      - Only the **immediate child** elements of the container become flex items. Children of flex items are not affected
  - With both flex-container and flex-item multiple CSS properties that can be added to these elements to control
    - the dimensions, alignment, spacing, arrangement, responsiveness(behaviour based on screensize) //TODO: add as may as possible to this list.
   
### Flex properties
- `justify-content:` used to control **spacing** of the flex items in the direction they are placed
  - flex-start(default), flex-end, center, space-between, space-around, space-evenly
  - ![image](https://github.com/connectkushal/cssnotes/assets/19621775/8165b1a9-4b7e-4558-8d6c-1e961a8d1d15)

- `flex-wrap`: based on screen size, whether to wrap content if space runs out.
  - `nowrap`(default), `wrap`, `wrap-reverse`

- `align-items:` used to control the alignment of flex items in their perpendicular direction.
  - useful when the height of each item is different
  - stretch(default), center, flex-start, flex-end, baseline
  - ![image](https://github.com/connectkushal/cssnotes/assets/19621775/d31b64e9-579c-45fe-8a6d-51b96c78b301)

- `flex-direction`
  - `row`(default), `column`, `row-reverse`, `column-reverse`
