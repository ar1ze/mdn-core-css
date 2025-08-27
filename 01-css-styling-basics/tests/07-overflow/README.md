# Test Your Skills: Overflow 📝
***
This skill test helps you understand and manage `overflow` in CSS.

### **In this article**
* Task 1
* Task 2

## Task 1 🎯
***
The goal is to fix overflowing content in a box with a fixed height.

### **Problem**
Content overflows a box with a fixed height.

### **Solution**
Update the CSS so that scrollbars appear only when necessary.

### **Code Snippet**
`html <div class="box"> <p> Veggies es bonus vobis, proinde vos postulo essum magis kohlrabi welsh onion daikon amaranth tatsoi tomatillo melon azuki bean garlic. </p> <p> Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot courgette tatsoi pea sprouts fava bean collard greens dandelion okra wakame tomato. Dandelion cucumber earthnut pea peanut soko zucchini. </p> </div>`

`css body { font: 1.2em / 1.5 sans-serif; } .box { border: 5px solid black; padding: 1em; height: 200px; width: 300px; }`

### **Answer**
Add `overflow: auto` to the `.box` selector.
`css .box { overflow: auto; }`

## Task 2 🖼️
***
The goal is to hide an image that is larger than its containing box.

### **Problem**
An image overflows its box, making it visibly larger than the container.

### **Solution**
Update the CSS to hide any part of the image that is outside the box.

### **Code Snippet**
`html <div class="box"> <img alt="flowers" src="https://mdn.github.io/shared-assets/images/examples/flowers.jpg" /> </div>`

`css body { font: 1.2em / 1.5 sans-serif; } .box { border: 5px solid black; height: 200px; width: 300px; }`

### **Answer**
Add `overflow: hidden` to the `.box` selector.
`css .box { overflow: hidden; }`