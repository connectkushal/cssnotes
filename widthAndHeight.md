### Width
- the width is set based on value of the `box-model` property
  - by default, for block elements it is measured for the `content` part
  - for `border-box`, it is measured for the total of `border+padding+content` (excluding margins)
- Block level elements have default width of `auto`
- other values in `percentage`, `px`, `em`, `rem`
  - in case of `%` value, the width is the percentage of its parent element


### Height
- general practice is not to set the height
- every element has an intrinsic height by default
  - the default height is calculated based on the basis of the contents of the element
- recomended to set `min-height` instead of fixed `height` (content controls the height)
  - element's height will grow if needed to avoid content overflow, like in mobile view of the website
  - example usecase, columns of same height with different content height
- *** If required to enlarge the background height, modify using `padding` instead

