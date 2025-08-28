# **Test Your CSS Skills: Floats** 💻

-----

### **Overview**

This skill test helps you assess your understanding of **floats** in CSS, including the `float` and `clear` properties, as well as other methods for clearing floats. It includes three small tasks covering different concepts.

  - **Note:** For help, read the **Test your skills usage guide** or use one of the communication channels.

### **Tasks**

-----

#### **Task 1: Floating Elements** ➡️⬅️

**Goal:** Float two elements (`.float1` and `.float2`) to the left and right, respectively, so that text appears between them.

**HTML:**

```html
<div class="box">
  <div class="float float1">One</div>
  <div class="float float2">Two</div>
  <p>The two boxes should float to either side of this text.</p>
</div>
```

**CSS Solution:**

```css
.float1 {
  float: left;
}

.float2 {
  float: right;
}
```

-----

#### **Task 2: Clearing Floats** 🧹

**Goal:** Float an element (`.float`) to the left. Make the first line of text appear next to it, but force the second line (`.below`) to display underneath the floated element.

**HTML:**

```html
<div class="box">
  <div class="float">Float</div>
  <p>This sentence appears next to the float.</p>
  <p class="below">Make this sentence appear below the float.</p>
</div>
```

**CSS Solution:**

```css
.float {
  float: left;
}

.below {
  clear: left;
}
```

-----

#### **Task 3: Containing Floats** 📦

**Goal:** Use a modern method to make the background of a container box (`.box`) extend below a floated element, instead of displaying behind it.

**HTML:**

```html
<div class="box">
  <div class="float">Float</div>
  <p>This sentence appears next to the float.</p>
</div>
```

**CSS Solution:**

The most up-to-date method is `display: flow-root;`. Other methods include using `overflow` or a `clearfix` hack.

```css
.box {
  display: flow-root;
}
```