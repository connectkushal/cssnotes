### Inheritance

1. Anything related to **typography** is inherited
  - `font-size, font-family, text-decoration, color, etc`
  - because of this it is common to place such rules on `body` or `html` tag
  - ![{F0C68D81-AEB7-4841-A29D-9696A1BF4099}](https://github.com/user-attachments/assets/4a0874e8-d5e0-4c74-9e04-56b0bed11dd4)
  - Browser defaults are **NOT** inherited
2. Nothing related to **layout** is inherited
  - `margin, padding, height, width, position`
3. Of the remaining elements, these do not inherit by default, they use browser defaults
  - `<button>` `<input>` `<optgroup>` `<select>` `<textarea>` // form related
  - when we want to make them inherit, use `font-family: inherit;`
  - ![{6679A4A1-CFEE-4A8A-9D33-7127C7D57569}](https://github.com/user-attachments/assets/251f2e56-d7be-4db0-9c3e-ccc96f035097)
