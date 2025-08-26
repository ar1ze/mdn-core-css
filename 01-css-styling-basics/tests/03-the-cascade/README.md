## Test Your Skills: The Cascade 📝

-----

### **Aim of the Test** 🎯

  * Assess understanding of universal property values for controlling inheritance in CSS.

### **Task 1** 🖌️

  * **Objective**: Use a special value to reset the background color to white without using an actual color value.
  * **Original CSS**:
    ```css
    #outer div ul .nav a {
      background-color: powderblue;
      padding: 5px;
      display: inline-block;
      margin-bottom: 10px;
    }

    div div li a {
      color: rebeccapurple;
    }
    ```
  * **Solution**:
    ```css
    #outer #inner a {
      background-color: inherit;
    }
    ```
  * **Explanation**:
      * The solution uses a more specific selector (`#outer #inner a`) to override the original rule.
      * The `inherit` keyword sets the background color to be the same as its parent element.

### **Task 2** 🎨

  * **Objective**: Manipulate cascade layer order to color links `rebeccapurple`.
  * **Context**: This task requires knowledge of **cascade layers**.
  * **Original CSS**:
    ```css
    @layer yellow, purple, green;

    @layer yellow {
      #outer div ul .nav a {
        padding: 5px;
        display: inline-block;
        margin-bottom: 10px;
      }
    }
    @layer purple {
      div div li a {
        color: rebeccapurple;
      }
    }
    @layer green {
      a {
        color: lightgreen;
      }
    }
    ```
  * **Solution**:
    ```css
    @layer yellow, green, purple;
    ```
  * **Explanation**:
      * Change the layer precedence by moving the `purple` layer to the end.
      * Styles in later-declared layers take precedence over styles in earlier-declared layers.