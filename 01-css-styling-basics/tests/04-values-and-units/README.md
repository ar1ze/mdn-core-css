# Test your skills: Values and units 🧪

-----

The aim of this skill test is to help you assess whether you understand different types of values and units used in CSS properties.

## Task 1: Color values 🎨

-----

In this task, the first list item has been given a background color using a hex color code. Complete the CSS using the same color in different formats.

  - **Objective:** Recreate a hex color (`#86defa`) using different color formats for different list items.
      - Second list item: Use **RGB** color.
      - Third list item: Use **HSL** color.
      - Fourth list item: Use **RGB** color with an **alpha channel** of `0.6`.

**Source HTML:**

```html
<ul>
  <li class="hex">hex color</li>
  <li class="rgb">RGB color</li>
  <li class="hsl">HSL color</li>
  <li class="transparency">Alpha value 0.6</li>
</ul>
```

**Solution CSS:**

```css
.hex {
  background-color: #86defa;
}

.rgb {
  background-color: rgb(134 222 250);
}

.hsl {
  background-color: hsl(194 92% 75%);
}

.transparency {
  background-color: rgb(134 222 250 / 60%);
}
```

## Task 2: Font sizes 📏

-----

In this task, we want you to set the font size of various items of text.

  - **Objective:** Set the font size for different elements using various units.
      - `<h1>`: `50px`
      - `<h2>`: `2em`
      - All `<p>` elements: `16px`
      - A `<p>` element directly after an `<h1>`: `120%`

**Source HTML:**

```html
<h1>Level 1 heading</h1>
<p> ... </p>
<h2>Level 2 heading</h2>
<p> ... </p>
```

**Solution CSS:**

```css
h1 {
  font-size: 50px;
}

h2 {
  font-size: 2em;
}

p {
  font-size: 16px;
}

h1 + p {
  font-size: 120%;
}
```

## Task 3: Background image position 🖼️

-----

To complete the task, update the CSS to move the background image so that it is centered horizontally and is 20% from the top of the box.

  - **Objective:** Use `background-position` to center an image horizontally and position it 20% from the top.

**Source HTML:**

```html
<div class="box"></div>
```

**Solution CSS:**

```css
.box {
  background-image: url("...");
  background-repeat: no-repeat;
  background-position: center 20%;
}
```