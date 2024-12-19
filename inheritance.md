### [< Index](https://github.com/connectkushal/cssnotes/tree/main?tab=readme-ov-file#index)
---

### Inheritance

- Anything related to **typography** is inherited
  - `font-size, font-family, text-decoration, color, etc`
  - because of this it is common to place such rules on `body` or `html` tag
  - ```css
    html {
      font-family: 'some-font', sans-serif;
      font-size: 1.125rem;
      font-weight: 400;
      line-height: 1.7;
    }
    ```
  - Browser defaults are **NOT** inherited
    
- Nothing related to **layout** is inherited
  - `margin, padding, height, width, position`
     
- Of the remaining elements, these do not inherit by default, they use browser defaults
  - `<button>` `<input>` `<optgroup>` `<select>` `<textarea>` // form related
  - when we want to make them inherit a property like line height, fonts, etc, use `font-family: inherit;`
  - ```css
    button, input, optgroup, select, textarea {
      font-family: inherit;
    }
    ```
- other ways to use inherit
  - ```css
    a {
      color: inherit;
    }
    ```
  - ```css
    h2, h3, h4 {
      font-weight: inherit;
    }
    ```
### misc notes
- on chorme, size of h1 inside `article` `aside` `nav` `section` is overridden by user-agent style sheet. Set `h1` properties explicitly to use own style.
  - ```css
    body {
      font-size: 1.125rem; // will not be inherited by h1 in chrome
    }

    h1 {
      font-size: 6rem;
    }
    ```
