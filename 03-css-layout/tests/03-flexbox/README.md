## Test Your Skills: Flexbox 📚

-----

The aim of this skill test is to help you assess whether you understand how **flexbox and flex items behave**. Below are four sets of design problems you can solve using flexbox. Your task is to fix the problems.

-----

### **Interactive Challenge** 💻

First, a fun, interactive flexbox challenge created by our learning partner, Scrimba. Watch the embedded scrim, and complete all the tasks on the timeline.

-----

### **Task 1** 🎯

  * **Problem:** Lay out list items for a site's navigation as a row with equal space between each item.
  * **HTML:**
    ```html
    <nav>
      <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/about">About Us</a></li>
        <li><a href="/products">Our Products</a></li>
        <li><a href="/contact">Contact Us</a></li>
      </ul>
    </nav>
    ```
  * **Solution:** Use `display: flex` and the `justify-content` property.
    ```css
    nav ul {
      display: flex;
      justify-content: space-between;
    }
    ```

-----

### **Task 2** 🎯

  * **Problem:** Display list items of different sizes as three equal-sized columns.
  * **HTML:**
    ```html
    <ul>
      <li>I am small</li>
      <li>I have more content than the very small item.</li>
      <li>I have lots of content. So much content that I don't know where it is all going to go. I'm glad that CSS is pretty good at dealing with situations where we end up with more words than expected!</li>
    </ul>
    ```
  * **Solution:**
    ```css
    ul {
      display: flex;
    }

    li {
      flex: 1;
    }
    ```
  * **Bonus Question:** Make the first item twice the size of the others.
  * **Bonus Solution:**
    ```css
    li:first-child {
      flex: 2;
    }
    ```

-----

### **Task 3** 🎯

  * **Problem:** Arrange list items into rows.
  * **HTML:**
    ```html
    <ul>
      <li>Turnip</li>
      <li>greens</li>
      <li>yarrow</li>
      <li>ricebean</li>
      <li>rutabaga</li>
      <li>endive</li>
      <li>cauliflower</li>
      <li>sea lettuce</li>
      <li>kohlrabi</li>
      <li>amaranth</li>
    </ul>
    ```
  * **Solution:** Requires understanding the `flex-wrap` property to wrap flex lines.
    ```css
    ul {
      display: flex;
      flex-wrap: wrap;
    }

    li {
      flex: auto;
    }
    ```

-----

### **Page Information** 📄

  * **Last Modified:** ⁨Aug 12, 2025⁩ by MDN contributors.
  * **Source:** View this page on GitHub.