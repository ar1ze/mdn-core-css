# **What is CSS?** 🎨

-----

### **Overview**

  * **CSS (Cascading Style Sheets)** allows you to create great-looking web pages.
  * This article explains what CSS is, its basic syntax, and how browsers apply it to HTML.

### **Prerequisites & Learning Outcomes**

  * **Prerequisites:** Basic software, file handling knowledge, and HTML familiarity.
  * **Learning Outcomes:**
      * The purpose of CSS.
      * HTML is separate from styling.
      * The concept of default browser styles.
      * What CSS code looks like.
      * How CSS is applied to HTML.

### **Browser Default Styles** 💻

-----

  * Browsers have **default styles** to make pages readable even without explicit styling from an author.
  * These styles are defined in default CSS stylesheets inside the browser, separate from HTML.

### **What is CSS For?** ✨

-----

  * CSS gives you control over how HTML elements look.
  * You can present documents with a custom design and layout.
  * **A document** is usually a text file structured with a markup language like HTML.
  * **Rendering** is the process of converting a document into a visually usable form in a browser.
  * **A user agent** is another term for a browser.
  * **Common uses for CSS:**
      * Text styling (color, size)
      * Creating layouts (grids, columns)
      * Special effects (animation)
  * The CSS language is organized into **modules** with related functionality.

### **CSS Syntax Basics** 📝

-----

  * CSS is a **rule-based language**.
  * You define **rules** to apply styles to elements.
  * **Example Rule:**
    ```css
    h1 {
      color: red;
      font-size: 2.5em;
    }
    ```
  * **Components of a rule:**
      * **Selector:** Selects the HTML element to style (e.g., `h1`).
      * **Declarations:** Contained within curly braces `{}`.
      * **Property and Value Pairs:** A declaration consists of a property (e.g., `color`) and a value (e.g., `red`), separated by a colon `:`.

### **How CSS is Applied to HTML** 🌳

-----

1.  The browser receives the HTML document and converts it to a **DOM tree**.
2.  Any CSS rules are sorted into "buckets" based on their selectors.
3.  The rules are applied to the DOM tree, creating a **render tree**.
4.  The render tree is then painted to the browser window.

<!-- end list -->

  * **Example:** Two `<p>` elements will both receive the same styling from a single `<p>` CSS rule.

### **Play with Some CSS** 🕹️

-----

  * You can use the MDN Playground editor to practice.
  * **Practice tasks:**
      * Add a new paragraph to see the CSS rule automatically apply.
      * Add an `<h2>` heading and create a new rule to style it.
      * Look up and experiment with new CSS properties from the **MDN CSS reference**.

### **Summary** 🚀

-----

  * This article provided a basic understanding of what CSS is and how it works.
  * The next step is to practice writing CSS yourself.