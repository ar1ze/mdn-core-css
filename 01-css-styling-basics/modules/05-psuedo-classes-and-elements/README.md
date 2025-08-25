# 📜 Pseudo-classes and Pseudo-elements

---

## 🧐 What are Pseudo-classes?

A **pseudo-class** is a selector that targets an element based on its specific state. It acts as if you applied a class to an element, helping to reduce excess classes in your HTML.

* They are keywords that start with a single colon (`:`).
* **Example:** `:hover` selects an element when the user's pointer is over it.
* **User-action pseudo-classes** (dynamic pseudo-classes) apply when a user interacts with the document, like `:hover` and `:focus`.

## ✍️ What are Pseudo-elements?

**Pseudo-elements** behave similarly to pseudo-classes but act as if you had added a completely new HTML element into the markup.

* They start with a double colon (`::`).
* **Example:** `::first-line` selects the first line of a text block, even if the line length changes.
* **Note:** Older pseudo-elements sometimes use a single colon (`:`) for backward compatibility.

---

## 🔗 Combining Pseudo-classes and Pseudo-elements

You can **chain** pseudo-classes and pseudo-elements together to create more specific selectors.

* **Syntax Example:** `article p:first-child::first-line` selects the first line of the first paragraph inside an `<article>` element.

## ➕ Generating Content

The `::before` and `::after` pseudo-elements are used with the **`content`** property to insert content into the document using CSS. This is called **generated content**.

* **Syntax:** `::before` inserts content at the beginning of an element, and `::after` inserts it at the end.
* **Common uses:**
    * Inserting strings of text (though this is not always accessible).
    * Adding icons or visual indicators.
    * Creating empty shapes that can be styled with CSS.

---

## 📝 Summary

* **Pseudo-classes (`:`)**: Select elements in a specific state.
* **Pseudo-elements (`::`)**: Select and style parts of an element as if they were new elements.
* The `::before` and `::after` pseudo-elements can be used with the `content` property to **generate content** via CSS.