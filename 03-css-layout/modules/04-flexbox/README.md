# Flexbox 📦


Flexbox is a one-dimensional layout method for arranging items in rows or columns. Items flex to fill or shrink to fit spaces.

---

## Prerequisites & Learning Outcomes 🎯

* **Learning Outcomes:**
    * Purpose of flexbox (one-dimensional layout).
    * Flex terminology (container, item, main/cross axis).
    * Understanding `display: flex`.
    * Wrapping content.
    * Flexible sizing and ordering.
    * Justifying and aligning content.

---

## Core Concepts 🧠

### **Specifying Flexboxes**

* Apply `display: flex;` to a parent element.
* The parent becomes a **flex container**.
* Its children become **flex items**.
* `display: flex;` makes the container a block-level element. `display: inline-flex;` makes it inline.

### **The Flex Model (Axes)**

* **Main axis**: Direction items are laid out (`row` or `column`).
    * Main start & main end.
    * Main size.
* **Cross axis**: Perpendicular to the main axis.
    * Cross start & cross end.
    * Cross size.

### **Direction & Wrapping**

* `flex-direction`: Sets the main axis direction.
    * `row` (default)
    * `column`
    * `row-reverse`
    * `column-reverse`
* `flex-wrap`: Controls overflow.
    * `nowrap` (default, items overflow container)
    * `wrap` (items wrap onto new lines)
* **Shorthand:** `flex-flow: <flex-direction> <flex-wrap>;`

### **Flexible Sizing**

* The `flex` property is a shorthand for `flex-grow`, `flex-shrink`, and `flex-basis`.
    * `flex: <flex-grow> <flex-basis>;` (e.g., `flex: 1 100px;`)
    * `flex-grow`: Unitless proportion of available space to take up.
    * `flex-shrink`: How much an item will shrink to prevent overflow (advanced).
    * `flex-basis`: The minimum size of an item before the remaining space is distributed.
* **Recommendation:** Use the `flex` shorthand property.

### **Alignment**

* `align-items`: Controls alignment along the **cross axis**.
    * `stretch` (default)
    * `center`
    * `flex-start`
    * `flex-end`
    * `baseline`
* `justify-content`: Controls alignment along the **main axis**.
    * `flex-start` (default)
    * `flex-end`
    * `center`
    * `space-around` (even space around items)
    * `space-between` (even space between items)
* `align-self`: Overrides `align-items` for an individual item.

### **Ordering**

* The `order` property changes the visual order of items without affecting the source code order.
* Default `order` is `0`.
* Higher values appear later; lower values appear earlier.
* **Note:** Changing order can negatively impact accessibility for keyboard users as the tabbing order remains the same as the source code.

### **Nested Flexboxes** 🌳

* A flex item can also be a flex container.
* This allows for the creation of complex layouts.

---

## Further Resources 📚

* [Basic concepts of flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout/Basic_concepts_of_flexbox)
* [CSS-Tricks guide to flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
* [Flexbox Froggy](https://flexboxfroggy.com/) (an educational game)