# Chapter 03: Colors

🎨 — CSS offers many ways to represent and use **colors** in styling.

---

## 🔑 1. **Named Colors**

CSS comes with around **140 predefined color names**.

```css
h1 {
  color: red;       /* keyword */
}
p {
  background-color: lightblue;
}
```

✅ Examples: `red`, `blue`, `green`, `orange`, `purple`, `black`, `white`.

---

## 🔑 2. **Hexadecimal Colors**

Hex codes are written as `#RRGGBB`.

* `RR` → red
* `GG` → green
* `BB` → blue
  (Each value from `00` to `FF` in hex = 0–255 in decimal)

```css
h1 {
  color: #ff0000;   /* pure red */
}
p {
  color: #00ff00;   /* pure green */
}
div {
  background: #0000ff; /* pure blue */
}
```

✅ Shorthand: `#RGB`

* `#f00` → red
* `#0f0` → green
* `#00f` → blue

---

## 🔑 3. **RGB Colors**

Defined with **decimal values** (0–255).

```css
p {
  color: rgb(255, 0, 0);   /* red */
}
div {
  background: rgb(0, 255, 0); /* green */
}
```

✅ You can also use **percentages**:

```css
color: rgb(100%, 0%, 0%); /* red */
```

---

## 🔑 4. **RGBA Colors (with Transparency)**

Same as RGB but with an **alpha channel** (`0.0` = fully transparent, `1.0` = fully opaque).

```css
div {
  background-color: rgba(255, 0, 0, 0.5); /* semi-transparent red */
}
```

---

## 🔑 5. **HSL Colors**

HSL = **Hue, Saturation, Lightness**

* **Hue**: angle on color wheel (0–360, 0 = red, 120 = green, 240 = blue)
* **Saturation**: 0% (gray) → 100% (full color)
* **Lightness**: 0% (black) → 50% (normal color) → 100% (white)

```css
p {
  color: hsl(0, 100%, 50%);    /* red */
}
div {
  background: hsl(120, 100%, 25%); /* dark green */
}
```

---

## 🔑 6. **HSLA Colors (with Transparency)**

Like HSL but with an alpha channel.

```css
div {
  background-color: hsla(240, 100%, 50%, 0.3); /* semi-transparent blue */
}
```

---

## 🔑 7. **Current Color Keyword**

Uses the element’s **current text color** for other properties.

```css
button {
  color: darkblue;
  border: 2px solid currentColor; /* same as text color */
}
```

---

## 🔑 8. **Gradients (Color Transitions)**

Gradients are treated as **images**, but they use colors.

```css
div {
  background: linear-gradient(to right, red, yellow);
}
```

* **Linear gradients**: top → bottom, left → right, etc.
* **Radial gradients**: circular or elliptical.

```css
background: radial-gradient(circle, blue, white);
```

---