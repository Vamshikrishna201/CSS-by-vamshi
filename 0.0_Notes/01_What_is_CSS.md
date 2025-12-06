# What is CSS?

- CSS stands for Cascading Style Sheets.
- CSS is the Language we use to style webpages.
- CSS save a lot of work, it can controll layout of myltiple web all at once.
- External stylesheets are stored in css files.

---

### CSS Syntax ->

```css
selector {
  property: value;
}
```

*example*

```css
h1 {
  color: red;
  font-size: 30px;
}
```

---

# How to add CSS

- There are 3 ways, but we use **ONLY ONE** in real Project

1. External Css - (Real Projects Use This)
2. Internal Css - Not mandatory
3. Inline Css - Not mandatory

---

### 1. External Css _Example_

```html
<link rel="stylesheet" href="style.css">
```
This is the correct/clean way.

> **NOTE:** Always use external CSS in real projects.

### 2. Internal Css _Example_

```html
<!DOCTYPE html>
<html>
<head>
    <title>Internal CSS Example</title>
    <style>
        /* CSS rules go here */
        h1 {
            color: #333;
            text-align: center;
        }
    </style>
</head>
<body>
    <h1>Welcome to My Page</h1>
</body>
</html>
```
### 3. Inline Css _Example_

```html
<h1 style="color: blue; text-align: center;">This is a Blue, Centered Heading</h1>
```
---

### CSS Boiler Plate Code

- CSS boilerplate reset -> a small piece of code, you add at the start to make your layout clean and predictable.

```css
/* Universal selection */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-mox;
}

html,body{
    width: 100%;
    height: 100%;
}
```