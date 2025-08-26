# Test your skills: The box model 📦

-----

## **Goal** 🎯

The aim of this skill test is to help you assess whether you understand the CSS box model.

## **Interactive Challenge** 💻

  * **Description:** A fun, interactive challenge involving margin shorthand.
  * **How to:** Watch the embedded scrim and complete the tasks on the timeline by editing the code.

-----

## **Task 1: The Alternate Box Model** 📏

  * **Objective:** Change the width of the second box (`.alternate`) to match the visual width of the first box.
  * **Initial HTML:**
    ```html
    <div class="box">I use the standard box model.</div>
    <div class="box alternate">I use the alternate box model.</div>
    ```
  * **Initial CSS:**
    ```css
    body { font: 1.2em / 1.5 sans-serif; }
    .box {
      border: 5px solid rebeccapurple;
      background-color: lightgray;
      padding: 40px;
      margin: 40px;
      width: 300px;
      height: 150px;
    }
    .alternate { box-sizing: border-box; }
    ```
  * **Solution:** Increase the width of the second block to add the size of the padding and border.
    ```css
    .alternate {
      box-sizing: border-box;
      width: 390px;
    }
    ```

-----

## **Task 2: Margin, Border, and Padding** 📝

  * **Objective:** Add specific styling features to the provided box.
  * **Required Features:**
      * A 5px, black, dotted border.
      * A top margin of 20px.
      * A right margin of 1em.
      * A bottom margin of 40px.
      * A left margin of 2em.
      * Padding on all sides of 1em.
  * **Initial HTML:**
    ```html
    <div class="box">I use the standard box model.</div>
    ```
  * **Initial CSS:**
    ```css
    body { font: 1.2em / 1.5 sans-serif; }
    .box { }
    ```
  * **Solution:** Use shorthand properties for margin, border, and padding.
    ```css
    .box {
      border: 5px dotted black;
      margin: 20px 1em 40px 2em;
      padding: 1em;
    }
    ```

-----

## **Task 3: Displaying Inline-Block** 📜

  * **Objective:** Update the CSS to make the lines above and below the inline element respect its margin, padding, and border, while keeping the element inline.
  * **Problem:** The inline element's margin, padding, and border are causing lines to overlap.
  * **Initial HTML:**
    ```html
    <div class="box">
      <p> Veggies es bonus vobis, <span>proinde vos postulo</span> essum magis kohlrabi welsh onion daikon amaranth tatsoi tomatillo melon azuki bean garlic. </p>
      <p> Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot courgette tatsoi pea sprouts fava bean collard greens dandelion okra wakame tomato. Dandelion cucumber earthnut pea peanut soko zucchini. </p>
    </div>
    ```
  * **Initial CSS:**
    ```css
    body { font: 1.2em / 1.5 sans-serif; }
    .box span {
      background-color: pink;
      border: 5px solid black;
      padding: 1em;
    }
    ```
  * **Solution:** Use `display: inline-block` to respect block direction margin, border, and padding.
    ```css
    .box span {
      background-color: pink;
      border: 5px solid black;
      padding: 1em;
      display: inline-block;
    }
    ```