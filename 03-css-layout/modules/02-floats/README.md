# Floats 🌊

Originally for floating images inside blocks of text, the **`float` property** became one of the most common tools for creating multiple column layouts. With the advent of **flexbox** and **grid**, it has returned to its original purpose.

-----

## Learning Outcomes 🎯

  * Understand the purpose of floats for floating images, drop caps, and inset information boxes.
  * Recognize that floats were previously used for multi-column layouts but are now considered a **legacy technique**.
  * Learn how to use the `float` property.
  * Learn how to clear floats using **`clear`** and **`display: flow-root`**.

-----

## The Background of Floats 📜

The `float` property was introduced to allow for image-in-text layouts, similar to what you'd see in a newspaper. Developers quickly realized it could be applied to any element, leading to its use for multi-column website layouts. However, newer, better techniques are now available, and floats should be reserved for their original purpose.

-----

## A Float Example 🛠️

To see how `float` works, follow these steps:

1.  **Start with HTML:**
    ```html
    <h1>Float example</h1>
    <div class="box">Float</div>
    <p>Lorem ipsum dolor sit amet...</p>
    <p>Sed auctor cursus massa...</p>
    <p>Nam vulputate diam...</p>
    ```
2.  **Add basic CSS:**
    ```css
    body {
      width: 90%;
      max-width: 900px;
      margin: 0 auto;
      font: 0.9em/1.2 Arial, Helvetica, sans-serif;
    }
    .box {
      width: 150px;
      height: 100px;
      border-radius: 5px;
      background-color: rgb(207 232 220);
      padding: 1em;
    }
    ```
3.  **Float the box:** Add `float: left;` and `margin-right: 15px;` to the `.box` rule. The `<div>` is taken out of normal flow and content wraps around it. Floating to the right has the same effect in reverse.

-----

## Visualizing the Float 👀

A floated element is removed from normal flow, and the boxes of following elements actually run **behind** it. To visualize this, add a `background-color` to a paragraph following a floated box. You'll see the background extends underneath the float, even though the text wraps around it.

-----

## Clearing Floats 🧹

To prevent an element from moving up alongside a float, use the **`clear` property**.

  * **Values:**
      * `clear: left;` : Clears items floated to the left.
      * `clear: right;` : Clears items floated to the right.
      * `clear: both;` : Clears any floated items.

-----

## Clearing Boxes Wrapped Around a Float 🎁

A common issue is when a parent container's background runs behind a float inside it. This happens because the float is taken out of the normal document flow and no longer contributes to the height of its parent.

  * **Solution:** Use **`display: flow-root;`** on the parent element. This property exists specifically to solve this issue without hacks.