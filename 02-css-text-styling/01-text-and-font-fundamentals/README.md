### 📝 Fundamental Text and Font Styling

---

### **Overview**

This article covers the fundamentals of styling text and fonts with CSS. It includes setting **font weight**, **family**, and **style**, using **shorthand**, and controlling **text alignment** and **spacing**.

* **Prerequisites:** Basic knowledge of HTML content structuring and CSS styling.
* **Learning Outcomes:**
    * Understanding font families, stacks, and web-safe fonts.
    * Setting font properties like **color**, **weight**, **size**, and **style**.
    * Controlling text layout with alignment, transform, and decoration.
    * Setting line height and other spacing properties.

---

### **What is Involved in Styling Text?**

Text flows within an element's **content box**. Text styling properties fall into two categories:

* **Font styles:** Properties that affect the font itself (e.g., `font-family`, `font-size`).
* **Text layout styles:** Properties that control spacing and alignment (e.g., `letter-spacing`, `text-align`).

---

### **Fonts**

#### **Color**

The `color` property sets the foreground color, which is usually the text. It accepts any CSS color unit.

**Example:** `p { color: red; }`

#### **Font Families**

The `font-family` property specifies a font or a list of fonts. The browser uses the first available font from the list.

* **Web Safe Fonts:** A limited set of fonts available on most systems. Examples include **Arial**, **Times New Roman**, and **Verdana**.
* **Default Fonts:** CSS defines five generic families: `serif`, `sans-serif`, `monospace`, `cursive`, and `fantasy`. These serve as a fallback.
* **Font Stacks:** It's best practice to provide a list of fonts and end with a generic font family as a fallback.

**Example:** `p { font-family: "Trebuchet MS", Verdana, sans-serif; }`

#### **Font Size**

The `font-size` property can be set using various units, but the most common are:

* **`px` (pixels):** An absolute unit.
* **`em`:** Relative to the parent element's font size.
* **`rem`:** Relative to the root `<html>` element's font size.

`rem` is often preferred for easier calculations.

#### **Font Style, Weight, and Decoration**

* `font-style`: Controls italics. Values: `normal`, `italic`, `oblique`.
* `font-weight`: Controls boldness. Values: `normal`, `bold`, `lighter`, `bolder`, or numeric values (`100` - `900`).
* `text-transform`: Changes text case. Values: `none`, `uppercase`, `lowercase`, `capitalize`.
* `text-decoration`: Adds/removes lines. Values: `none`, `underline`, `overline`, `line-through`. This can also be a shorthand for multiple properties.

#### **Text Drop Shadows**

The `text-shadow` property adds shadows. It takes up to four values: **horizontal offset**, **vertical offset**, **blur radius**, and **color**. Multiple shadows can be applied by separating values with commas.

**Example:** `text-shadow: 4px 4px 5px red;`

---

### **Text Layout**

* `text-align`: Controls horizontal alignment. Values: `left`, `right`, `center`, `justify`.
* `line-height`: Sets the height of each line. A unitless value (e.g., `1.6`) is a multiplier of the font size and is generally recommended for readability.
* `letter-spacing` & `word-spacing`: Adjusts spacing between letters and words.

---

### **Font Shorthand**

The `font` shorthand property sets multiple font properties in a single declaration.

* **Order:** `font-style` `font-variant` `font-weight` `font-stretch` `font-size`/`line-height` `font-family`
* Only `font-size` and `font-family` are required.

**Example:** `font: italic bold 1.2em/1.5 Arial, sans-serif;`

---

### **Summary**

This guide provides a foundational understanding of CSS text and font styling, from basic properties like `color` and `font-family` to more advanced layout controls and shorthand properties.