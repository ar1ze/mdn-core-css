# Backgrounds and Borders 🎨

In this lesson, you'll learn about creative CSS styling using backgrounds and borders, including gradients, images, and rounded corners.

---

## Prerequisites & Learning Outcomes ✅

**Prerequisites:**

- HTML basics
- CSS Values and units
- CSS Sizing

**Learning Outcomes:**

- **Background Styling:** Colors, images, size, repeat, position, and attachment.
- **Gradients:** The general concept and linear gradients.
- **Accessibility:** Ensuring good contrast with backgrounds.
- **Borders:** Width, style, color, and border shorthand.
- **Rounded Corners:** Using the `border-radius` property.

---

## Key Concepts 💡

### Background Colors

- The `background-color` property sets the background color of any element.
- It accepts any valid `<color>` value.
- The color extends under the content and padding of the element.

### Background Images

- The `background-image` property displays an image in the background of an element.
- **Tiling Behavior:** Controlled by `background-repeat` with values like `no-repeat`, `repeat-x`, `repeat-y`, and `repeat`.
- **Sizing:** Managed with `background-size`. Keywords include `cover` (covers the entire area, may crop) and `contain` (fits inside the box, may leave gaps).
- **Positioning:** The `background-position` property uses a coordinate system (0,0) at the top-left corner. It accepts keywords, lengths, and percentages.

### Gradient Backgrounds

- Gradients act like images and are set using the `background-image` property.
- The `<gradient>` data type includes `linear-gradient()` and `radial-gradient()`.

### Multiple Backgrounds

- You can use multiple background images in one declaration by separating values with commas.
- The images are layered on top of each other in the order they're listed.
- Other `background-*` properties can also have comma-separated values that cycle through.

### Background Attachment

- The `background-attachment` property controls how backgrounds scroll with content.
- **`scroll`**: The background scrolls with the page.
- **`fixed`**: The background is fixed to the viewport.
- **`local`**: The background scrolls with the element's content.

### Background Shorthand

- The `background` shorthand property sets all background properties at once.
- Properties for multiple backgrounds are separated by commas.
- `background-color` must be the last value.
- `background-size` follows `background-position` with a slash (`/`).

### Accessibility with Backgrounds ♿

- Ensure sufficient contrast between text and background for legibility.
- Always specify a `background-color` as a fallback if the image fails to load.
- Background images should be purely decorative since screen readers cannot parse them.

### Borders

- The `border` shorthand property sets the width, style, and color for all four sides.
- Individual properties like `border-width`, `border-style`, and `border-color` can also be used.
- Specific sides can be targeted (e.g., `border-top`).

### Rounded Corners 🟢

- The `border-radius` property adds rounded corners to a box.
- It can accept one value for all corners or multiple values for specific corners.