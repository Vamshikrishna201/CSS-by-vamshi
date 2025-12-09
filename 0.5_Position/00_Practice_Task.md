# ✔ CSS Position — Understand It, Don’t Memorize

### 1. static (default)
-   Every element is **static** by default.
-   You **cannot move it** with `top`/`right`/`bottom`/`left`.
-   It takes the **normal document flow**.
-   👉 *Useless for layouts. It’s just the default mode.*

---

### 2. relative
-   Keeps the element in the **normal flow**.
-   But allows **shifting the element from its own original position**. 
-   *Example:*
    -   If you do `top: 10px`, it moves down 10px, but its space in the layout stays where it originally was.
-   👉 *Mental model: “It’s standing in its place, but you drag it a little.”*

--

### 3. absolute
-   **Removes the element from the normal flow.**
-   It no longer occupies space (its siblings act as if it's not there).
-   It positions itself relative to the **nearest ancestor that has a position other than static** (i.e., `relative`, `absolute`, or `fixed`).
-   If no such parent → it positions relative to the viewport.
-   👉 *Mental model: “A floating element that ignores all siblings.”*

--

### 4. fixed
-   Like absolute, **removed from flow**.
-   But **sticks to the viewport** always (scrolling won't affect its position). 
-   👉 *Common use: navbars, sticky buttons, floating icons.*

--

### 5. sticky
-   **Hybrid** between `relative` and `fixed`.
-   Behaves like **`relative`** until a scroll threshold is reached.
-   Then it becomes **`fixed`** until its container ends.
-   👉 *Used for sticky headers, sections, etc.*

---

# ✔ Your Practice Task (Simple but Powerful)

Don’t skip this; it forces you to actually understand.

## Task 1 — Relative + Absolute Positioning


#### Create a box like this:

- A parent <div> of width 200px, height 200px, background: lightgray.
- Inside it, create a small red box (50x50).
- Position the red box at the bottom-right corner using absolute.

But the parent must have `position: relative.`

(This is the core concept that most people fail at.)

---