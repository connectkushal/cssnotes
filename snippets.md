## Misc CSS snippets

generic html
```html
<div class="container">
  <div class="item">
      Center of the div
  </div>
</div>
```

- ### Centering a div
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

- ### Full page content
```css
.container{
  width: 100%;
  height: 100vh;
  background-color: somecolor;
}
```
