### Notes on css and sass

#### Index

- [Setup](#setup)
- [Introduction](https://github.com/connectkushal/cssnotes/blob/main/introduction.md)
- Basics
  - [Vocabulary](https://github.com/connectkushal/cssnotes/blob/main/vocabulary.md)
  - [Units](https://github.com/connectkushal/cssnotes/blob/main/units.md)
- Layouts
  - [Box Model](https://github.com/connectkushal/cssnotes/blob/main/boxmodel.md)
  - [Flexbox](https://github.com/connectkushal/cssnotes/blob/main/flexbox.md)
  - [Grid]() 
- [Snippets]()

 

---

##### Setup
- inside your project directory, run `npm init -y && npm pkg set type="module"`

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
