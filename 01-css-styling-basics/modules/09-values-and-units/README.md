# CSS Values and Units 📚

---

CSS rules use declarations with properties and **values**. Each property has a specific **value type** that dictates the kind of values it can accept. This document explores frequently used value types.

## Key Concepts 💡

---

* **CSS Values:** Define valid value types for each CSS property (e.g., `<color>`, `<length>`).
* **Data Types:** Interchangeable term for value types.
* **Angle Brackets (`<`, `>`):** Used in CSS specifications to denote a value type, distinguishing it from a property with a similar name.

## Numbers, Lengths, and Percentages 📏

---

### Numeric Value Types

* **`<integer>`**: A whole number (e.g., 1024, -55).
* **`<number>`**: A decimal number (e.g., 0.255, -1.2).
* **`<dimension>`**: A number with a unit (e.g., 45deg, 10px). This is a broad category including:
    * `<length>`
    * `<angle>`
    * `<time>`
    * `<resolution>`
* **`<percentage>`**: A fraction of another value, always relative (e.g., 50% of the parent element's length).

### Lengths

There are two types of length units:

* **Absolute Units**: Not relative to anything else; generally the same size.
    * **`px` (Pixels)**: The most common unit for screens. Note that 1px might span multiple physical device pixels.
    * **`cm`**, **`mm`**, **`Q`**, **`in`**, **`pc`**, **`pt`**: More useful for print media.
* **Relative Units**: Relative to something else, enabling scaling.
    * **`em`**: Relative to the current element's `font-size`.
    * **`rem`**: Relative to the root element's (`<html>`) `font-size`.
    * **`vh`** & **`vw`**: Relative to the viewport's height and width, respectively.

## Color 🎨

---

Color values can be set in many ways for properties like text, backgrounds, and borders. The standard system uses 24-bit colors, allowing for ~16.7 million distinct colors.

* **Color Keywords**: Named colors (e.g., `black`, `rebeccapurple`). Often used in examples for clarity but less common in production.
* **Hexadecimal RGB Values**: Use a hash symbol followed by six hex characters (e.g., `#ffc0cb`). Each pair represents Red, Green, and Blue channels.
* **RGB Values**: Use the `rgb()` function with three parameters (0-255 or 0-100%) for Red, Green, and Blue. An optional fourth parameter separated by a slash (`/`) specifies opacity.
* **Hue-based Colors**: Use hue as the primary component, often with a color wheel angle.
    * **`hwb()`**: Specifies color with Hue, Whiteness, and Blackness.
    * **`hsl()`**: Specifies color with Hue, Saturation, and Lightness.

## Other Value Types 📋

---

* **Images**: The `<image>` value type can be a file (via `url()`) or a **gradient** (e.g., `linear-gradient()`).
* **Position**: The `<position>` value type defines 2D coordinates. It can use keywords (`top`, `center`, `right`) or lengths to specify offsets for things like background images.
* **Strings and Identifiers**:
    * **Identifiers**: Unquoted keywords that CSS understands (e.g., `red`).
    * **Strings**: Quoted values used for specifying content (e.g., `content: "Hello World";`).
* **Functions**: Pieces of code that perform a specific task, such as `rgb()`, `hsl()`, and `calc()`.
    * **Math Functions**: Allow calculations within CSS (e.g., `calc(20% + 100px)`).

## Summary ✨

---

This overview covers the most common CSS value and unit types. Each property has a defined list of allowed value types. Understanding these types is crucial for effective styling and layout.