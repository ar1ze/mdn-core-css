# **📝 Styling Lists with CSS**

-----

This article explains how to style lists using CSS, covering spacing, bullet types, and custom images. Lists, for the most part, behave like other text, but some properties are specific to them.

## **📋 Prerequisites & Learning Outcomes**

  * **Prerequisites**: Basic knowledge of structuring content with HTML and CSS.
  * **Learning Outcomes**:
      * Spacing list items with properties like `margin` and `line-height`.
      * Using `list-style` properties to control bullets.

## **🛒 A Simple List Example**

-----

The article uses HTML examples for unordered, ordered, and description lists to demonstrate styling.

### **Default Browser Styles**

  * `<ul>` and `<ol>`: Default top/bottom `margin` of `16px` (`1em`) and `padding-left` of `40px` (`2.5em`).
  * `<li>`: No default spacing.
  * `<dl>`: Top/bottom `margin` of `16px` (`1em`), but no padding.
  * `<dd>`: Default `margin-left` of `40px` (`2.5em`).

## **📏 Handling List Spacing**

-----

The goal is to maintain a consistent **vertical rhythm** with surrounding elements.

  * Set consistent `font-size` for headings, lists, and paragraphs.
  * Apply the same `line-height` to list items and paragraphs.
  * For description lists, set a `line-height` for `<dd>` and `<dt>` elements and use `font-weight: bold` on `<dt>` to make them stand out.

## **✒️ List-Specific Styles**

-----

Three main properties for styling list bullets on `<ul>` or `<ol>` elements:

  * `list-style-type`: Defines the type of bullet (e.g., `square`, `circle`, `upper-roman`, `lower-alpha`).
    ```css
    ol {
      list-style-type: upper-roman;
    }
    ```
  * `list-style-position`: Sets whether bullets appear `inside` or `outside` the list item content. The default is `outside`.
  * `list-style-image`: Allows a custom image to be used as the bullet. This property is less flexible than using background properties.

### **Using Background Properties for Custom Bullets**

For more control, use `background` properties on `<li>` elements:

1.  Set `list-style-type: none` to remove the default bullet.
2.  Use `background-image: url(...)` to insert the custom bullet.
3.  Control the bullet's position with `background-position`, size with `background-size`, and repetition with `background-repeat: no-repeat`.

### **`list-style` Shorthand**

The three properties can be combined into a single shorthand property:
`list-style: square url("example.png") inside;`

## **🔢 Controlling List Counting**

-----

HTML attributes can modify ordered list counting:

  * `start`: Starts the list from a number other than 1.
    ```html
    <ol start="4">...</ol>
    ```
  * `reversed`: Makes the list count backward.
    ```html
    <ol start="4" reversed>...</ol>
    ```
  * `value`: Sets a specific numerical value for an individual `<li>` element.
    ```html
    <li value="2">...</li>
    ```

## **🧩 Styling a Nested List (Task)**

-----

The article provides a practical task to style a nested list, with a solution provided at the end. The task involves:

1.  Styling the unordered list with `square` bullets.
2.  Giving all `<li>` items a `line-height` of `1.5`.
3.  Setting the ordered list to have `lower-alpha` bullets.

### **✅ Solution**

```css
ul {
  list-style-type: square;
}

li {
  line-height: 1.5;
}

ol {
  list-style-type: lower-alpha;
}
```