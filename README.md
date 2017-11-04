# CSS align a required field asterisk correctly before or after a form label text

```html
  <div class="form-group">
    <label class="required" for="username">Username</label>
    <input class="form-control" type="text" value="" name="username" id="username" required>
  </div>

  <div class="form-group">
    <label class="required-after" for="email">Email</label>
    <input class="form-control" type="email" value="" name="email" id="email" required>
  </div>
```

```css
  label.required:before {
    color: red;
    content: "*";
    font-size: 20px;
    position:relative;
    top:6px;
    font-family: arial;
  }
  
  label.required-after:after {
    color: red;
    content: " *";
    font-size: 20px;
    position:relative;
    top:6px;
    font-family: arial;
  }
```

See it on [Fiddle](https://jsfiddle.net/victorybiz/pvsxc5x0/)
