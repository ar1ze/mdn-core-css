# Test Your Skills: Selectors 🚀

-----

The aim of this skill test is to help you assess whether you understand **CSS selectors**. To complete these tasks, you should only edit the CSS, not the HTML.

## Task 1 🎯

  - Make `<h1>` headings **blue**.
  - Give `<h2>` headings a **blue background** and **white text**.
  - Cause text wrapped in a `<span>` to have a `font-size` of **200%**.

### Solution:

```css
h1 {
  color: blue;
}

h2 {
  background-color: blue;
  color: white;
}

span {
  font-size: 200%;
}
```

## Task 2 🏷️

  - Give the element with an **id of `special`** a **yellow background**.
  - Give the element with a **class of `alert`** a **2px solid grey border**.
  - If the element with a class of `alert` also has a **class of `stop`**, make the background **red**.
  - If the element with a class of `alert` also has a **class of `go`**, make the background **green**.

### Solution:

```css
#special {
  background-color: yellow;
}

.alert {
  border: 2px solid grey;
}

.alert.stop {
  background-color: red;
}

.alert.go {
  background-color: green;
}
```

## Task 3 🔗

  - Style links, making the **link-state orange** and **visited links green**.
  - **Remove the underline** on hover.
  - Make the **first element inside the `container`** `font-size: 150%`.
  - Make the **first line of that element red**.
  - **Stripe every other row** in the table with a background color of `#333333` and foreground **white**.

### Solution:

```css
.container p:first-child {
  font-size: 150%;
}

.container p:first-child::first-line {
  color: red;
}

a:link {
  color: orange;
}

a:visited {
  color: green;
}

a:hover {
  text-decoration: none;
}

tr:nth-child(even) {
  background-color: #333333;
  color: white;
}
```

## Task 4 ➡️

  - Make any paragraph that **directly follows an `<h2>`** element **red**.
  - Remove the bullets and add a **1px grey bottom border** only to list items that are a **direct child of the `<ul>`** with a class of `list`.

### Solution:

```css
h2 + p {
  color: red;
}

.list > li {
  list-style: none;
  border-bottom: 1px solid #cccccc;
}
```

## Task 5 ✨

  - Target the `<a>` element with a **`title` attribute** and make the border **pink**.
  - Target the `<a>` element with an **`href` attribute that contains `contact`** and make the border **orange**.
  - Target the `<a>` element with an **`href` value starting with `https`** and give it a **green border**.

### Solution:

```css
a[title] {
  border-color: pink;
}
a[href*="contact"] {
  border-color: orange;
}
a[href^="https"] {
  border-color: green;
}
```