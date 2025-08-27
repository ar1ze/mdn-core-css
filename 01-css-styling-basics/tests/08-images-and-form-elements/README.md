# Test Your Skills: Images and Form Elements 📝

---

The purpose of this test is to assess your understanding of how CSS treats special elements like images, media, and form elements.

### Task 1: Image Overflow 🖼️
- **Goal:** Scale an image to fit inside a box without extra white space, cropping if necessary.
- **Problem:** An image is overflowing its container.
- **Solution: **
  - Add `height: 100%` and `width: 100%` to the `img` element.
  - Use `object-fit: cover` to crop the image to fit the container.

### Task 2: Form Styling with Attribute Selectors 💻
---
- **Goal:** Style a basic search form using attribute selectors.
- **Requirements:**
  1.  Target the search field and submit button within `.my-form` using attribute selectors.
  2.  Set the text size of the form field and button to match the rest of the form (`font-size: inherit`).
  3.  Give both elements `10px` of padding.
  4.  Style the button with a `rebeccapurple` background, `white` text, no border, and a `5px` `border-radius`.

### Task 3: Advanced Form Styling and Layout 📐
---
- **Goal:** Implement a form with consistent styling and a neat layout.
- **Requirements:**
  1.  Apply a lightweight CSS reset for consistent fonts, padding, and sizing.
  2.  Add consistent styling for inputs and the button.
  3.  Use a layout technique (like Flexbox) to align labels and inputs neatly.
- **CSS Solution Breakdown:**
  - `* { box-sizing: border-box; }`: A common reset for consistent sizing.
  - `button, input, select { ... }`: Resets form elements' font, padding, and margin to be consistent.
  - `li { display: flex; align-items: center; ... }`: Uses Flexbox to align labels and inputs horizontally within each list item.
  - `label { flex: 0 40%; ... }`: Sets the label to take up 40% of the flex container's space and aligns text to the right.
  - `input, select { flex: auto; ... }`: Allows the input fields to fill the remaining space.
  - `input, select, button { ... }`: Applies consistent padding, border, and border-radius.
  - `button { ... }`: Centers the button and adds a background color.
  - `button:hover, button:focus { ... }`: Adds a hover/focus state for better user experience.