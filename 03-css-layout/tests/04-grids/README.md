# Test Your Skills: CSS Grids 🧠

The goal of this skill test is to assess your understanding of how CSS Grid and grid items function. It consists of several small tasks that apply concepts from the material covered.

-----

## Task 1: Auto-Placing Items 🗺️

**Objective:** Create a grid with four child elements that auto-place. The grid should have three equally-spaced columns and a 20px gap between rows and columns.

### HTML

```html
<div class="grid">
  <div>One</div>
  <div>Two</div>
  <div>Three</div>
  <div>Four</div>
</div>
```

### CSS Solution

```css
.grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 20px;
}
```

-----

## Task 2: Spanning & Layering Items 🎭

**Objective:** Edit CSS to make two child elements span across multiple grid tracks. The second item should overlay the first.

**Bonus:** Make the first item display on top without changing its order in the HTML.

### HTML

```html
<div class="grid">
  <div class="item1">One</div>
  <div class="item2">Two</div>
</div>
```

### CSS Solution

```css
.item1 {
  grid-column: 1 / 4;
  grid-row: 1 / 3;
}

.item2 {
  grid-column: 2 / 5;
  grid-row: 2 / 4;
}
```

### Bonus Solution

```css
/* Option 1: Using 'order' */
.item1 {
  order: 1;
}

/* Option 2: Using 'z-index' */
.item1 {
  z-index: 1;
}
```

-----

## Task 3: Layout with Named Areas 🏷️

**Objective:** Use `grid-area` and `grid-template-areas` properties to lay out four children according to a specific design.

### HTML

```html
<div class="grid">
  <div class="one">One</div>
  <div class="two">Two</div>
  <div class="three">Three</div>
  <div class="four">Four</div>
</div>
```

### CSS Solution

```css
.grid {
  display: grid;
  gap: 20px;
  grid-template-columns: 1fr 2fr;
  grid-template-areas: "aa aa" "bb cc" ". dd";
}

.one {
  grid-area: aa;
}

.two {
  grid-area: bb;
}

.three {
  grid-area: cc;
}

.four {
  grid-area: dd;
}
```

-----

## Task 4: Combining Grid and Flexbox 🧩

**Objective:** Recreate a card layout using both **Grid** and **Flexbox**. The gap between columns and rows should be 10px.

### HTML

```html
<div class="container">
  <div class="card">
    <img alt="a single red balloon" src="https://mdn.github.io/shared-assets/images/examples/balloons1.jpg" />
    <ul class="tags">
      <li>balloon</li>
      <li>red</li>
      <li>sky</li>
      <li>blue</li>
      <li>Hot air balloon</li>
    </ul>
  </div>
  ... (additional cards)
</div>
```

### CSS Solution

```css
.container {
  display: grid;
  gap: 10px;
  grid-template-columns: 1fr 1fr 1fr;
}

.tags {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
```