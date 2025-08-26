# Sizing Items in CSS 📏

---

## What is Sizing in CSS?

This lesson summarizes how elements are sized in CSS and defines key terms.

**Prerequisites:**

* HTML basics
* CSS basic syntax
* CSS selectors

**Learning Outcomes:**

* Understand the concept of **intrinsic size**.
* Learn about setting **absolute and percentage sizes**.
* Understand **`min-` and `max-` sizes**.
* Learn about **viewport units** and their usefulness.

---

## Intrinsic vs. Extrinsic Sizing 📐

* **Intrinsic Size**: The natural size of an element before any CSS is applied.
    * An image's intrinsic size is determined by its file's dimensions.
    * An empty `<div>` has no intrinsic size of its own; its height is defined by its content.

* **Extrinsic Size**: A specific size that is explicitly given to an element using CSS.
    * This can cause **overflow** if the content is larger than the assigned size.
    * Fixing heights with lengths or percentages should be done carefully to avoid overflow issues.

---

## Sizing with Percentages and Units 📊

### Percentages

* Percentages act like length units and can be used interchangeably.
* A child element's percentage width is relative to the **parent container's width**.
* **Percentage margins and padding** are calculated from the **inline size (width)** of the containing block, not the height. This allows for equal-sized margins and padding on all four sides.

### Min- and Max- Sizes

* **`min-height`**: Ensures an element is at least a certain height, but allows it to grow taller if more content is added, preventing overflow.
* **`max-width`**: A common use case is for **responsive images**.
    * Setting `width: 100%` can cause a small image to stretch and become pixelated.
    * Using `max-width: 100%` ensures the image scales down to fit a smaller container but won't stretch to become larger than its intrinsic size.

### Viewport Units 🖥️

* Units that relate to the size of the user's browser viewport.
* **`vw`** (viewport width): `1vw` is equal to 1% of the viewport width.
* **`vh`** (viewport height): `1vh` is equal to 1% of the viewport height.
* Useful for creating elements that are sized relative to the user's screen.
    * For example, a hero section with `height: 100vh` will fill the entire screen height.