# 📝 Styling Tables with CSS

---

This article explains how to make HTML tables look good using specific CSS techniques.

## 📋 Prerequisites & Learning Outcomes

---

**Prerequisites:**
- Basic HTML syntax & HTML tables
- CSS Values & units
- Sizing

**Learning Outcomes:**
- Handling table spacing & border collapsing.
- Highlighting different table regions (`<thead>`, `<tbody>`, `<tfoot>`, `<caption>`).
- Implementing zebra striping for improved readability.

## 🛠️ Getting Started

---

1.  Start with the provided sample HTML markup for a table of punk bands.
2.  Create a `style.css` file in the same directory.
3.  Link the CSS file to the HTML using `<link href="style.css" rel="stylesheet" />` inside the `<head>`.

## 🎨 Core Styling Techniques

---

### 1. Font Update
- Use `font-family: Arial, Helvetica, sans-serif;` for a less formal look.

### 2. Spacing
- Use `table-layout: fixed;` to make table behavior more predictable.
- Set `width: 80%;`, `min-width: 1000px;`, and `margin: 0 auto;` for a responsive, centered table.
- Use `border-collapse: collapse;` to merge table borders into a single line.
- Add `padding: 0.6em;` to `<th>` and `<td>` elements to give content space.

### 3. Alignment
- Align text to the left and numbers to the right.
- Use the `:nth-child` pseudo-class to select and style specific columns.
- Set specific widths on columns, giving more space to text-heavy columns.
- Use `vertical-align: top;` on `<th>` and `<td>` to align content to the top of cells.

### 4. Adding Borders
- Add borders to visually separate the table caption, data, and footer.
- Use `border-top: 1px solid #999999;` on `<tfoot>` and `<table>` and `border-bottom: 1px solid #999999;` on `<table>`.

### 5. Zebra Striping
- Use `tbody tr:nth-child(odd) { background-color: #eeeeee; }` to alternate row colors, making the table easier to read. `odd` is a shortcut for the `2n+1` formula.

### 6. Styling the Caption
- Use `caption-side: bottom;` to position the caption at the bottom of the table.

## 🎯 Quick Tips for Table Styling

---

- Keep markup simple and flexible.
- Use `table-layout: fixed;` and `border-collapse: collapse;`.
- Use `<thead>`, `<tbody>`, and `<tfoot>` for logical structure and easy styling.
- Implement **zebra striping** for readability.
- Use `text-align` to align content properly.