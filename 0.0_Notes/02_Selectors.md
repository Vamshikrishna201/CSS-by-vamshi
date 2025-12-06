# What is CSS Selectors

- CSS selectors are used to *find (or select)* the HTML element you want to style

- We can divide CSS selectors into 5 categories

### 1. Element Selector (used for global styles)

```css
p {
  font-size: 16px;
}
```
---

### 2. Class Selector (MOST USED)

```css
.box {
  color: red;
}
```
---

### 3. ID Selector (rare, but useful for unique elements)

```css
#header {
  background: black;
}
```
---

### 4. Descendant Selector (very useful!)

```css
.nav a {
  color: blue;
}
```

- Means: inside `.nav`, style only `a` tags.

---

### 5. Pseudo-elements Selectors (Select and style a part of a element)

```css

```

## ⭐ IMPORTANT NOTE 2:

- Use class almost always.
- Use ID only when you truly need it (forms, JS).




