# **Positioning in CSS**

---

This article explains how to use the **`position`** property to control the layout of elements, moving them out of the normal document flow.


## **Key Concepts** 💡

The `position` property has different values that change an element's behavior:

* **`static` (Default):** Elements are positioned in their normal flow. Using `top`, `bottom`, `left`, or `right` has no effect.
* **`relative`:** Elements remain in the normal flow, but their final position can be adjusted using `top`, `bottom`, `left`, and `right`. This moves the element relative to its original position, potentially causing it to overlap other elements.
* **`absolute`:** Elements are taken **completely out** of the normal document flow and positioned relative to their nearest **positioned ancestor**. If no ancestor has a `position` other than `static`, the element is positioned relative to the initial containing block (the viewport).
* **`fixed`:** Similar to `absolute`, but the element is positioned relative to the **viewport** and stays in place even when the page is scrolled. This is useful for elements like persistent navigation menus.
* **`sticky`:** A hybrid of `relative` and `fixed`. The element behaves as `relative` until it reaches a specified scroll threshold, at which point it becomes `fixed`.

## **Controlling Position & Stacking** ↕️

* **`top`, `bottom`, `left`, `right`:** These properties are used with `relative`, `absolute`, and `fixed` positioning to specify an element's final location. The effect is different for each position type.
* **`z-index`:** This property controls the stacking order of **positioned elements** on the z-axis (perpendicular to the screen). A higher `z-index` value places an element on top of elements with lower values. By default, positioned elements have `z-index: auto` (effectively 0), and elements later in the source order appear on top.

## **Summary** ✨

Basic positioning is not ideal for entire layouts but is powerful for specific tasks like creating unique visual effects, overlaying UI elements (e.g., popups, menus), and fixing elements in place on the screen.