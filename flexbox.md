### [< Index](https://github.com/connectkushal/cssnotes/tree/main?tab=readme-ov-file#index)
---

### General

#### normal flow of document
- elements are positioned on a page according to
  - the order in which they are written in the HTML
  - and whether their **behavior is inline or block**
    - one below the other for block-level elements
    - one next to the other for inline or inline-block level elements.
  - margins and padding used to control the space between the elements
- `position:` , `display:`, `float:` used to create layout before flex //TODO: example code.

  ### Example code
  
  ### Flexbox Concept
  - Flexbox is a method to arrange elements **in one direction**, horizontally or vertically.
  - Flexbox system has a **Flex Container** which has within it **Flex Item**
    - **flex container** is the parent element.
    - There should be **at least one** child element or **flex item**
  - It is important to note that only the **immediate child** elements of the container become flex items. Children of flex items are not affected
  - With both flex-container and flex-item multiple CSS properties that can be added to these elements to control
    - the dimensions, alignment, spacing, arrangement, responsiveness(behaviour based on screensize) //TODO: add as may as possible to this list.
   
### Flex properties
#### Container
- `display: flex`: makes the element a flexbox container
  - the container itself will behave as a block element
- `display: inline-flex`: container behaves as an inline element
- `flex-direction`
  - `row`(default), `column`, `row-reverse`, `column-reverse`

- `flex-wrap`: based on screen size, whether to wrap content if space runs out.
  - `nowrap`(default), `wrap`, `wrap-reverse`

- `justify-content:` used to control **spacing** of the flex items in the direction they are placed
  - flex-start(default), flex-end, center, space-between, space-around, space-evenly
  - ![image](https://github.com/connectkushal/cssnotes/assets/19621775/8165b1a9-4b7e-4558-8d6c-1e961a8d1d15)

- `align-items:` used to control the alignment of flex items in their perpendicular direction which is called `cross-axis`.
  - useful when the height of each item is different
  - stretch(default), center, flex-start, flex-end, baseline
  - ![image](https://github.com/connectkushal/cssnotes/assets/19621775/d31b64e9-579c-45fe-8a6d-51b96c78b301)
 
- `align-content`: for setting alignment of content that is multi-row, eg with wrap. // find more use cases

#### Container properties shorthand
- `flex-flow`: is a shorthand for setting both direction and wrap.
  - default is `row nowrap` 

#### Items
- `flex-grow`
  
- `flex-shrink`: set the propotion wrt initial size, at which the element with shrink acording to screen size
  - `1`(default), `0` for no shrinking.
    
- `flex-basis`
  - `auto`(default) : the size is auto-calculated based on the properties **width** or **height**
  - other value can be in `% , px , em or rem` similar to the width and height properties.
  - The value can also be a keyword such as `min-content`, `fill` and so on
    
- `align-self`: overrides the align-items property of the parent container for the flex-item it is applied to
  - values same as `align-item`
    
- `margin` and `margin-*`: where * can be top, bottom, left or right
  - this can be used to extend margins to occupy the extra space
  - `auto`,
    
- `order`:
  - `0`(default), to any number
 
// TODO: find behaviour of the combination of values for flex-wrap, flex-grow, flex-shrink and flex-basis.
