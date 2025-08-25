# Basic CSS Selectors 🎯

This article recaps fundamental CSS selectors, including **type**, **class**, and **ID selectors**, **selector lists**, and the **universal selector**. It's a foundational guide for anyone styling HTML documents.

-----

## 🧐 What is a Selector?

A **CSS selector** is the first part of a CSS rule. It's a pattern that tells the browser which HTML elements to select and apply styles to. The selected elements are the **subject** of the selector.

-----

## 🏷️ Type Selectors

Also known as **tag name** or **element selectors**, these select HTML tags directly.

  * Example: `span`, `em`, `strong`, `h1`

<!-- end list -->

```css
span { 
  background-color: yellow; 
}

strong {
  color: rebeccapurple;
}
```

-----

## ✍️ Class Selectors

The **case-sensitive** class selector starts with a dot (`.`). It selects all elements with that class applied.

  * Example: `.highlight`

<!-- end list -->

```css
.highlight { 
  background-color: yellow; 
}
```

### Targeting Classes on Specific Elements

You can target a specific element with a class by combining the element's type selector with the class selector (e.g., `span.highlight`).

```css
span.highlight { 
  background-color: yellow; 
}

h1.highlight { 
  background-color: pink; 
}
```

### Multiple Classes

You can apply multiple classes to an element and chain them together in a selector to match only when all are present (e.g., `.notebox.warning`).

```css
.notebox { 
  border: 4px solid #666666; 
}

.notebox.warning { 
  border-color: orange; 
}
```

-----

## 🆔 ID Selectors

The **case-sensitive** ID selector begins with a hash (`#`). It is similar to a class selector but has a key difference:

  * An **ID must be unique** and used only once per page.
  * Elements can only have a single `id` value.

<!-- end list -->

```css
#one {
  background-color: yellow;
}

h1#heading {
  color: rebeccapurple;
}
```

> **⚠️ Warning:** Using the same ID multiple times in a document is invalid code and can cause unexpected behavior.

-----

## 📝 Selector Lists

If multiple selectors share the same CSS declarations, they can be combined into a comma-separated list.

  * Example: `h1, .special`

<!-- end list -->

```css
h1, .special {
  color: blue;
}
```

> **❗️ Note:** If any selector in the list is invalid, the entire rule will be ignored.

-----

## 🌐 The Universal Selector

The **universal selector** is an asterisk (`*`) and selects everything in the document.

  * Example: `*`

<!-- end list -->

```css
* {
  margin: 0;
}
```

This is often used in "reset stylesheets" to remove default browser styling. It can also improve readability when chained with a pseudo-class, like `article *:first-child`.