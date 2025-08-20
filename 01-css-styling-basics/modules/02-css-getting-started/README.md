# **Getting Started with CSS** 🚀

-----

This article will teach you how to apply CSS to a simple HTML document and introduce you to fundamental CSS syntax and features.

### **Prerequisites & Learning Outcomes** 🧠

-----

  * **Prerequisites:** Basic software, file management, and HTML knowledge.
  * **Learning Outcomes:**
      * Applying CSS to an HTML document.
      * Writing basic CSS.
      * Using fundamental selectors and combinators.
      * Understanding CSS state.
      * Familiarity with `@rules`, functions, shorthand properties, and whitespace.

### **Starting with HTML** 📝

-----

The starting point is a basic HTML document. You can save the following code as `index.html`:

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <title>Getting started with CSS</title>
</head>
<body>
  <h1>I am a level one heading</h1>
  <p>This is a paragraph of text. In the text is a <span>span element</span> and also a <a href="https://example.com">link</a>.</p>
  <p>This is the second paragraph. It contains an <em>emphasized</em> element.</p>
  <ul>
    <li>Item <span>one</span></li>
    <li>Item two</li>
    <li>Item <em>three</em></li>
  </ul>
</body>
</html>
```

### **Applying CSS** 🎨

-----

There are three ways to apply CSS to an HTML document:

1.  **External Stylesheets:**

      * The most common method.
      * Create a separate `.css` file (e.g., `styles.css`).
      * Link it in your HTML `<head>` with `<link rel="stylesheet" href="styles.css" />`.
      * Allows styling multiple pages with a single file.

2.  **Internal Stylesheets:**

      * CSS rules are placed within `<style>` tags inside the HTML `<head>`.
      * Useful for single pages or when you cannot modify external files.
      * Less efficient for multi-page sites as styles must be repeated.

3.  **Inline Styles:**

      * CSS declarations are placed directly on an HTML element using the `style` attribute.
      * Example: `<span style="color: purple; font-weight: bold">span element</span>`.
      * **Bad practice** as it mixes code and content, making maintenance difficult. Avoid when possible.

### **Common Selectors** 🎯

-----

  * **Element Selectors:** Target all elements of a specific type (e.g., `p`, `h1`).
  * **Multiple Selectors:** Target several elements by separating them with a comma (e.g., `p, li`).
  * **Class Selectors:** Target a specific subset of elements. Add a `class` attribute to the HTML and use a period in the CSS (e.g., `<li class="special">` becomes `.special { ... }`).
  * **Descendant Combinator:** Styles an element based on its parent (e.g., `li em` styles `<em>` elements that are inside an `<li>`).
  * **Next-Sibling Combinator:** Styles an element that directly follows another (e.g., `h1 + p` styles a `<p>` that comes right after an `<h1>`).
  * **State-based Styling:** Styles elements based on their state using pseudo-classes (e.g., `a:link`, `a:visited`, `a:hover`).
      * `a:hover { text-decoration: none; }` is a common example.
      * **Accessibility Note:** Be careful not to remove cues like underlines that help users identify links.

### **Other CSS Syntax Features** 🧩

-----

  * **Functions:** Values that take the form of a function name followed by parentheses.
      * `calc()`: Performs simple math (e.g., `width: calc(90% - 30px);`).
      * `rotate()`: A value for the `transform` property (e.g., `transform: rotate(0.8turn);`).
  * **`@rules`:** Provide instructions on how CSS should behave.
      * `@media`: Used for media queries, applying styles based on conditions like viewport width (e.g., `@media (width >= 30em)`).
  * **Shorthand Properties:** Combine multiple related properties into a single line.
      * Examples: `padding`, `margin`, `background`, `font`.
      * `padding: 10px 15px 15px 5px;` is a shorthand for four separate `padding` properties.
  * **Comments:** Begin with `/*` and end with `*/`.
      * Used to explain code or "comment out" sections for testing.
  * **Whitespace:** Browsers ignore extra whitespace (spaces, tabs, new lines).
      * Use it to make your code readable and well-structured.
      * **Caution:** Don't remove spaces within property names or values where they are required (e.g., `0 auto` is valid, but `0auto` is not).