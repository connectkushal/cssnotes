### Notes on css and sass

#### Index
- [Setup](#setup)
- [Units](#units)
 

---

##### Setup 
without build tools
- `npm i -g sass`
- `sass -w input.scss output.css` running on the terminal
- vscode plugin liveserver from `index.html`

##### Setup with vite
- `npm i -g vite sass`
- to index.html, add link:css with href=`path/to/main.scss` or `app.scss`
- `vite run dev`
  - OR run `vite run build` then liveserver plugin

---
#### Units
- 1em = browser default font size (usually 16px)
- 
  |em   |px  |
  |-----|----|
  |0.125|6   |
  |0.5  |8   |
  |0.625|10  |
  |0.75 |12  |
  |0.875|14  |
  |**1**    |**16**  |
  |1.125|18  |
  |1.25 |20  |
  |1.375|22  |
  |1.5  |24  |
  |1.625|26  |
  |1.75 |28  |
  |1.875|30  |
  |2    |32  |
  |3    |48  |
