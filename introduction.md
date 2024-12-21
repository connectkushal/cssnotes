### [< Index](https://github.com/connectkushal/cssnotes/tree/main?tab=readme-ov-file#index)
---

### Introduction
- the structure of modern css is mostly guided by:
  - css has to be adaptive to website clients
    - websites to be device agnostic, responsive
    - consistent look and feel in contrasts, colors, typography
  - Clients controls configurations
    - browser types, fontsize, screen orientations, screen size, themes(dark/light)

- Keeping the above in mind, css should describe the intent instead of the outcome, which can be overridden by clients.
- Be aware of the relationships between
  - viewport and elements
  - parent and its element
  - sibling elements
  - Example
    - is an element defining width? is the parent defining the width ? is the child's width a percent of the parents? is it causing overflow
- The relationships is controlled/defined by a given elements **formatting context**
- Layouts are all about relationships between elements
  - css also has a tight relationship with html
- things to keep in mind are global scope, isolated scope
  - then comes design systems
