# Introduction to CSS Layout 🎨

-----

This lesson covers CSS layout features, including `display` values, and introduces concepts for this module. It also explains normal flow.

### Prerequisites 📚

  * Structuring content with HTML
  * CSS Styling basics
  * Fundamental text and font styling

### Learning Outcomes ✅

  * Recognize methods for modern page layouts.
  * Understand that normal flow is the default browser layout for block and inline content.
  * Know that properties like `display`, `float`, and `position` change content layout.

### CSS Page Layout Techniques 📐

  * Control element positioning relative to:
      * Default position in normal flow
      * Other elements
      * Parent container
      * Viewport/window
  * No single technique is for isolation; understanding each method's purpose helps in choosing the right one.

## In this Article 📖

  * Normal layout flow
  * How are elements laid out by default?
  * Overriding normal flow
  * Summary

## Normal Layout Flow 🌊

-----

  * Elements lay out in "normal flow" by default, without CSS changes.
  * Can be changed by adjusting their position or removing them from flow.
  * Starting with a solid, well-structured document ensures readability on limited browsers or screen readers.

### How are elements laid out by default? 📦

  * **Box Model:** Padding, border, and margin are added to an element's content.
  * **Block-level elements:**
      * Content fills available inline space of the parent.
      * Grows along the block dimension to accommodate content.
      * Appear on a new line below the last one.
      * Separated by margins.
  * **Inline-level elements:**
      * Size is just the size of their content.
      * Sit on the same line with adjacent text nodes as long as there is space.
      * Overflowing content wraps to a new line.
  * **Margin Collapsing:** If vertical margins of two adjacent elements touch, the larger margin remains and the smaller one disappears.

### Normal Flow Example 📄

```html
<h1>Basic document flow</h1>
<p>I am a basic block level element. My adjacent block level elements sit on new lines below me.</p>
<p>By default we span 100% of the width of our parent element, and we are as tall as our child content. Our total width and height is our content + padding + border width/height.</p>
<p>We are separated by our margins. Because of margin collapsing, we are separated by the size of one of our margins, not both.</p>
<p>Inline elements <span>like this one</span> and <span>this one</span> sit on the same line along with adjacent text nodes, if there is space on the same line. Overflowing inline elements will <span>wrap onto a new line if possible (like this one containing text)</span>, or just go on to a new line if not, much like this image will do: <img src="https://mdn.github.io/shared-assets/images/examples/long.jpg" alt="snippet of cloth" /></p>
```

```css
body {
  width: 500px;
  margin: 0 auto;
}

p {
  background: rgb(255 84 104 / 30%);
  border: 2px solid rgb(255 84 104);
  padding: 10px;
  margin: 10px;
}

span {
  background: white;
  border: 1px solid black;
}
```

  * HTML is displayed in the exact order it appears.
  * Block elements are stacked.
  * Starting with well-structured HTML is crucial before altering default behavior.

## Overriding Normal Flow 🚧

-----

### Methods to override normal flow:

  * **`display` property:**
      * Values like `block`, `inline`, or `inline-block` change how elements behave in normal flow.
  * **Floats:**
      * Applying `float` (`left`, `right`) causes block-level elements to wrap around one side, similar to text wrapping an image in a magazine.
  * **Positioning:**
      * The `position` property controls precise box placement.
      * `static` is the default.
      * Other values like `position: fixed` can fix an element to the viewport.
  * **Specific layout systems (via `display`):**
      * **CSS Grid:** Alters how child elements are laid out inside their parents.
      * **Flexbox:** Also alters how child elements are laid out inside their parents.
  * **Responsive design:**
      * Adapts layouts for different devices.
      * Uses the `@media` at-rule to apply different layouts based on screen width, resolution, etc.

### Other Layout Techniques (Less Common) 🧪

  * **Table layout:** `display: table` and associated properties can be used on non-table elements.
  * **Multi-column layout:** Properties that cause block content to lay out in columns (like a newspaper).

## Summary 📝

-----

This article provided a summary of key layout technologies. Next, we will cover floats in detail.