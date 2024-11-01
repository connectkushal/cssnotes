### [< Index](https://github.com/connectkushal/cssnotes/tree/main?tab=readme-ov-file#index)
---

### Misc CSS snippets

generic html
```html
<div class="container">
  <div class="item">
      Some random text content lorem ipsum et al
  </div>
</div>
```

- #### Centering a div
```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```
or
```css
.container {
  display: flex;
  justify-content: center;
}

.item {
  margin: auto;
}
```

- #### Full page content
```css
.container{
  width: 100%;
  height: 100vh;
  background-color: somecolor;
}
```
- #### Responsive page without flexbox
  ```css
  .container {
    margin: 0 auto;
    width: 80%
  }
  ```
