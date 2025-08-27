# 📝 Test Your Skills: Backgrounds and Borders

-----

## 🎯 Aim

The goal of this skill test is to evaluate your understanding of **backgrounds** and **borders** in CSS.

-----

## 🛠️ Task 1

### **Objective:**

Add a background, border, and some basic styles to a page header.

### **Instructions:**

  * **Border:** Add a **5px black solid border** with **10px rounded corners**.
  * **Heading:** Give the `<h2>` a **semi-transparent black background** and **white text**.
  * **Background Image:** Add a background image (`https://mdn.github.io/shared-assets/images/examples/balloons.jpg`) and size it to **cover the box**.

### **Solution Snippet:**

```css
.box {
  border: 5px solid black;
  border-radius: 10px;
  background-image: url("https://mdn.github.io/shared-assets/images/examples/balloons.jpg");
  background-size: cover;
}

h2 {
  background-color: rgb(0 0 0 / 50%);
  color: white;
}
```

-----

## 🎨 Task 2

### **Objective:**

Add background images, a border, and other styling to a decorative box.

### **Instructions:**

  * **Border:** Add a **5px lightblue border**, with the **top-left corner rounded by 20px** and the **bottom-right corner rounded by 40px**.
  * **Heading Background:** Use the `star.png` image (`https://mdn.github.io/shared-assets/images/examples/star.png`) as a background with **one centered star on the left** and a **repeating pattern of stars on the right**.
  * **Text Alignment:** Center the heading text and ensure it doesn't overlap the image.

### **Solution Snippet:**

```css
.box {
  border: 5px solid lightblue;
  border-top-left-radius: 20px;
  border-bottom-right-radius: 40px;
}

h2 {
  padding: 0 40px;
  text-align: center;
  background: url("https://mdn.github.io/shared-assets/images/examples/star.png") no-repeat left center, url("https://mdn.github.io/shared-assets/images/examples/star.png") repeat-y right center;
}
```

-----

## 🔗 Additional Resources

  * **Previous:** Overview: CSS styling basics
  * **Next:** (Link to next topic)

-----

## \<footer\>

  * **Last Modified:** ⁨Aug 21, 2025⁩
  * **Contributors:** MDN contributors