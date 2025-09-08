# Chapter 02: Selectors

CSS selectors are **patterns** that tell the browser *which elements* in the HTML document should be styled. They form the **"hook"** between your HTML and your CSS rules.

## 🔑 Types of CSS Selectors

### 1. **Universal Selector**

```css
* {
  margin: 0;
  padding: 0;
}
```

* Selects **all elements** on the page.

---

### 2. **Type Selector (Element Selector)**

```css
p {
  color: blue;
}
```

* Selects all `<p>` elements.

---

### 3. **Class Selector**

```css
.box {
  border: 1px solid black;
}
```

* Selects elements with `class="box"`.
* Can be reused on multiple elements.

---

### 4. **ID Selector**

```css
#header {
  background-color: gray;
}
```

* Selects an element with a unique `id="header"`.
* Each `id` should only appear once in the HTML.

---

### 5. **Group Selector**

```css
h1, h2, h3 {
  font-family: Arial, sans-serif;
}
```

* Applies the same style to multiple selectors.

---

### 6. **Descendant Selector (Space)**

```css
div p {
  color: green;
}
```

* Selects `<p>` inside a `<div>` (at any nesting level).

---

### 7. **Child Selector (`>`)**

```css
div > p {
  color: red;
}
```

* Selects `<p>` elements that are **direct children** of a `<div>`.

---

### 8. **Adjacent Sibling Selector (`+`)**

```css
h1 + p {
  color: orange;
}
```

* Selects the **first `<p>`** immediately after an `<h1>`.

---

### 9. **General Sibling Selector (`~`)**

```css
h1 ~ p {
  color: purple;
}
```

* Selects **all `<p>` siblings** that come after an `<h1>`.

---

### 10. **Attribute Selectors**

```css
input[type="text"] {
  border: 1px solid black;
}
```

* Matches elements by attributes.
  Other examples:

```css
a[target="_blank"] { color: red; }
a[href^="https"] { color: green; }   /* starts with */
a[href$=".pdf"] { color: blue; }     /* ends with */
a[href*="login"] { color: orange; }  /* contains */
```

---

### 11. **Pseudo-classes**

Apply styles in certain states.

```css
a:hover {
  color: red;
}
p:first-child {
  font-weight: bold;
}
```

---

### 12. **Pseudo-elements**

Style specific parts of an element.

```css
p::first-line {
  color: blue;
}
p::before {
  content: "👉 ";
}
```

---

## 📌 Specificity Order

If multiple selectors match, CSS decides which one "wins" based on **specificity**:

1. Inline styles (highest priority)
2. ID selectors (`#id`)
3. Class/attribute/pseudo-class selectors (`.class`, `[attr]`, `:hover`)
4. Element selectors (`div`, `p`)
5. Universal selector (`*`) (lowest priority)

---

✅ So in short:
CSS selectors let you **target exactly the HTML elements** you want to style, from the whole page down to a single letter.