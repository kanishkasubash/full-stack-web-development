# Chapter 01: Get Started

CSS stands for **Cascading Style Sheets**.
It’s a stylesheet language used to **control the presentation and design** of web pages. While **HTML** provides the structure and content of a webpage (like text, images, and links), **CSS describes how those elements should look**—their colors, sizes, layouts, spacing, fonts, and more.

## Key Points about CSS:

1. **Separation of concerns**

   * HTML = content & structure
   * CSS = styling & layout
     This separation makes websites easier to maintain and update.

2. **Selectors & Rules**
   CSS works by targeting HTML elements (using *selectors*) and applying styles (with *properties* and *values*).
   Example:

   ```css
   p {
     color: blue;
     font-size: 16px;
   }
   ```

   → This makes all `<p>` (paragraph) text blue with a font size of 16 pixels.

3. **Cascading nature**

   * Multiple styles can apply to the same element. CSS follows rules of priority:

     * Inline styles > Internal styles > External styles
     * More specific selectors override general ones.
     * Later rules override earlier ones if they have the same weight.

4. **Styling Capabilities**
   CSS can control:

   * Colors, fonts, and text styles
   * Spacing (margin, padding, line height)
   * Layouts (flexbox, grid, positioning)
   * Animations & transitions
   * Responsive design (adapts to different screen sizes)

5. **How it’s used**
   CSS can be added to a webpage in three ways:

   * **Inline** (inside an element’s `style` attribute)
   * **Internal** (inside a `<style>` tag in HTML)
   * **External** (linked `.css` file, best practice for large projects)

👉 In short, **CSS is what makes websites look attractive and usable**, turning plain HTML into a styled and user-friendly page.