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

with vite
- `npm i -g vite sass`
- to index.html, add link:css with href=`path/to/main.scss` or `app.scss`
- `vite run dev`
  - OR run `vite run build` then liveserver plugin
    
**Notes for vite setup**
- to avoid sass warning messages, add this config to `vite.config.js` 
    
    ```
    import { defineConfig } from 'vite'

    export default defineConfig({
      css: {
          preprocessorOptions: {
              scss: {
                  api: "modern"
              }
          }
      }
    })
    ```
   -  `import { defineConfig } from 'vite'` // this is for editor's intellisense
   -  `api: "modern"` // vite's options not part of sass-cli, the default is set to `"legacy"`
   -  other options used in vite to config sass, like `quietDeps:true` is actually `--quiet-deps` from the sass cli, check sass official docs accordingly.
- `package.json` should have `type="module"` to avoid warning messages from vite
    
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
