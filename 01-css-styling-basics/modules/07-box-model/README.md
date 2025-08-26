# 📦 The Box Model

Everything in CSS has a box around it. Understanding these boxes is key to creating complex layouts and aligning elements. This lesson covers the CSS Box Model, how it works, and related terminology.

***

### 📝 Prerequisites & Learning Outcomes

* **Prerequisites:** HTML basics (Basic HTML syntax).
* **Learning Outcomes:**
    * Block and inline elements.
    * The different boxes: content, margin, border, padding.
    * The alternative box model (`box-sizing: border-box`).
    * Margin collapsing.
    * Basic `display` values: `block`, `inline`, `inline-block`, `none`.

***

### 🧱 Block and Inline Boxes

* In CSS, boxes are categorized as **block boxes** or **inline boxes**.
* This refers to how a box behaves in page flow and in relation to other boxes.
* Boxes have an **inner display type** and an **outer display type**.

#### `display: block` 🟪

* Breaks onto a new line.
* `width` and `height` properties are respected.
* `padding`, `margin`, and `border` push other elements away.
* Defaults for elements like `<h1>` and `<p>`.

#### `display: inline` ➡️

* Does **not** break onto a new line.
* `width` and `height` properties are ignored.
* Top and bottom `padding`, `margin`, and `border` do not affect other inline boxes.
* Left and right `padding`, `margin`, and `border` do move other content.
* Defaults for elements like `<a>`, `<span>`, `<em>`, and `<strong>`.

***

### 📏 What is the CSS Box Model?

The box model applies to **block boxes** and defines how the parts of a box work together.

#### Parts of a Box:

1.  **Content Box:** 🖼️ Area where content is displayed (`width`, `height`).
2.  **Padding Box:** 🌬️ Whitespace around content (`padding`).
3.  **Border Box:** 🖼️ Wraps content and padding (`border`).
4.  **Margin Box:** ➡️ Outermost whitespace, pushes other elements away (`margin`).

#### Standard vs. Alternate Box Model

* **Standard Model (Default):**
    * `width` and `height` apply to the **content box**.
    * Padding and border are **added** to these dimensions.
    * Example: `width: 350px` + `padding: 25px` (left/right) + `border: 5px` (left/right) = **410px** total width.

* **Alternate Model (`box-sizing: border-box`):**
    * `width` and `height` apply to the **visible box** (content + padding + border).
    * Padding and border are **subtracted** from the content area.
    * Example: `width: 350px` = **350px** total width.

***

### 🛠️ Key Properties: Margins, Padding, and Borders

#### Margin ↔️

* Invisible space **around** the box.
* Pushes other elements away.
* Can have positive or negative values.
* Shorthand: `margin`. Longhands: `margin-top`, `margin-right`, `margin-bottom`, `margin-left`.
* **Margin Collapsing:** Vertical margins of two adjacent block elements will collapse into a single margin, equal to the largest of the two.

#### Borders 🖼️

* Drawn **between** the margin and padding.
* Can be styled with `width`, `style`, and `color`.
* Shorthand: `border`. Also specific shorthands like `border-top`.
* Most granular longhands: `border-top-width`, `border-top-style`, `border-top-color`, etc.

#### Padding 🌬️

* Space **between** the border and the content.
* Pushes content away from the border.
* Cannot have negative values.
* Background color/image extends behind the padding.
* Shorthand: `padding`. Longhands: `padding-top`, `padding-right`, `padding-bottom`, `padding-left`.

***

### 🕹️ `display: inline-block`

* A value that is a middle ground between `inline` and `block`.
* **Behaves like `inline`:** Does **not** break onto a new line.
* **Behaves like `block`:** **Respects** `width` and `height` properties, and `padding`, `margin`, and `border` cause other elements to move away.
* Useful for giving inline elements (like links) a larger, clickable area with padding.