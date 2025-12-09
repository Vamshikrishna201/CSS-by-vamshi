# ✔ FLEXBOX — THE ONLY NOTES ACTUALLY NEED

Flexbox is for **1-dimensional layout** (row or column). 

If you ever struggle with alignment, spacing, centering → you’re not using Flex correctly.
You control flex in two directions:

## ✔ Main Axis
-   Horizontal (if `flex-direction: row`)
-   Vertical (if `flex-direction: column`)

## ✔ Cross Axis
-   Perpendicular to the main axis.

---

## ✔ The Key Properties (Stop wasting time on useless ones)

### 1. display: flex
-   Turns the container into a flex container.

```css
.container {
  display: flex;
}
```

---

### 2. flex-direction

- Defines direction of children.

```css
row          (default)
row-reverse
column
column-reverse

```

You MUST understand that `justify-content` works on the main axis,
and `align-items` works on the cross axis.

---

### 3. justify-content

- Controls spacing along main axis.

```css
justify-content: flex-start;    // left
justify-content: center;        // center
justify-content: flex-end;      // right
justify-content: space-between;
justify-content: space-around;
justify-content: space-evenly;
```

If this doesn’t work → your flex-direction is wrong.

---

### 4. align-items

Controls alignment **across the cross axis.**

```css
align-items: flex-start;
align-items: center;
align-items: flex-end;
align-items: stretch;   // default
```

Most people confuse this with justify-content.

---

### 5. gap

Adds spacing between items (modern & clean).

```css
gap: 20px;
```

Stop using margin hacks.

---

### 6. flex-wrap

Allows items to wrap to the next line.

```css
flex-wrap: wrap;
```

Without wrap → items shrink and look ugly.

---

### 7. flex (shorthand)

This is for children, not the container.

It controls how items grow or shrink.

```css
flex: 1;  // take equal space
```

### THE ONLY FLEXBOX DIAGRAM YOU NEED

```sql
Main Axis (row)  → →
Cross Axis (column)
↑
|
|
↓
```

If direction changes → the axes flip.

---

### ✔ SIMPLE BUT PERFECT SAMPLE CODES

**1. Center an element perfectly**

This is what 90% developers keep googling:

```html
<!-- html -->
<div class="container">
  <div class="box">Center</div>
</div>
```
```css
/* css */
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 300px;
  background: lightgray;
}

.box {
  width: 100px;
  height: 50px;
  background: tomato;
}
```

---

### 2. Three boxes spaced evenly

```html
<!-- html -->
<div class="container">
  <div class="box"></div>
  <div class="box"></div>
  <div class="box"></div>
</div>

```
```css
/* css */
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
}

.box {
  width: 80px;
  height: 80px;
  background: royalblue;
}

```

### 3. Responsive wrapping card layout

This is real-useful.

```html
<!-- html -->
<div class="cards">
  <div class="card"></div>
  <div class="card"></div>
  <div class="card"></div>
  <div class="card"></div>
</div>


```
```css
/* css */
.cards {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}

.card {
  flex: 1 1 200px;  /* grow | shrink | base width */
  height: 150px;
  background: lightgreen;
}

```

---

## ✔ TASK 1 — Build a Dice (Real Dice Layout)

Use only **Flexbox** to place the dots.

**Requirements:**

Create a 200×200 white dice with black dots.
Build all six sides using flex.


**Example patterns (must match real dice):**

1️⃣ One dot → centered using flex

2️⃣ Two dots → top-left & bottom-right

3️⃣ Three dots → top-left, center, bottom-right

4️⃣ Four dots → four corners

5️⃣ Five dots → four corners + center

6️⃣ Six dots → three on left column + three on right column

Rules:

- Use display: `flex` + `justify-content` + `align-items`

- No absolute positioning

- No grid

- Every dot must be a 20×20 circle

If you cannot do this → your flex understanding is weak.

---

## ✔ TASK 2 — Instagram-style Profile Row

Create a horizontal row like Instagram user profile:

- Left: round profile picture

- Middle: username + bio stacked vertically

- Right: Follow button

Rules:

- Everything must be aligned center vertically

- Use flexbox only

- Use `gap` (not margin hacks)

- Follow button must stay on the right side using margin-left: auto;

This tests: **main axis + cross axis + auto margin** tricks

---


## ✔ TASK 3 — Responsive Pricing Cards

Create 3 pricing cards side-by-side:

- On large screens → display in a row

- On small screens → wrap into a column

- Use **flex-wrap: wrap**

- Cards must have equal height using `flex: 1`

This tests: **wrapping, spacing, equal-growth flex**.

---

## ✔ TASK 4 — Chat App UI (WhatsApp-like)

Create 10 chat messages:

- Current user messages → aligned right (green box)

- Other user messages → aligned left (gray box)

Rules:

- Use flexbox with `align-self: flex-end` for right side messages

- Container width: 300px

- Each message box has padding & border radius

- Use gap between messages

This tests: **cross-axis control + align-self + realistic layout**.

---

---
