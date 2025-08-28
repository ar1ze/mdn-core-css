# 📝 Test your skills: Positioning

-----

This skill test helps you assess your understanding of the CSS `position` property and its values.

## 🎯 Task 1

**Objective:** Position the element with the class `.target` to the top and right of its container.

**HTML:**

```html
<div class="container">
  <p> Veggies es bonus vobis, proinde vos postulo essum magis kohlrabi welsh onion daikon amaranth tatsoi tomatillo melon azuki bean garlic. </p>
  <div class="target">Target</div>
  <p> Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot courgette tatsoi pea sprouts fava bean collard greens dandelion okra wakame tomato. Dandelion cucumber earthnut pea peanut soko zucchini. </p>
</div>
```

**CSS (to complete):**

```css
.container { /* Add styles here */ }
.target { /* Add styles here */ }
```

**Solution:**
This task requires using `position: relative` on the container and `position: absolute` on the target. This creates a new positioning context.

```css
.container { 
  position: relative; 
}

.target { 
  position: absolute; 
  top: 0; 
  right: 0; 
}
```

**Bonus Question:**
Change the target to display underneath the text.

**Bonus Solution:**
Add a negative `z-index` to the target, e.g., `z-index: -2`.

## 🛠️ Task 2

-----

**Objective:** Update the code so that the sidebar (`<div class="sidebar">`) stays in place while only the content scrolls.

**HTML:**

```html
<div class="container">
  <div class="sidebar">
    <p> This is the sidebar. It should remain in position as the content scrolls. </p>
  </div>
  <div class="content">
    <p> Veggies es bonus vobis, proinde vos postulo essum magis kohlrabi welsh onion daikon amaranth tatsoi tomatillo melon azuki bean garlic. </p>
    <p> Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot courgette tatsoi pea sprouts fava bean collard greens dandelion okra wakame tomato. Dandelion cucumber earthnut pea peanut soko zucchini. </p>
    <p> Turnip greens yarrow ricebean rutabaga endive cauliflower sea lettuce kohlrabi amaranth water spinach avocado daikon napa cabbage asparagus winter purslane kale. Celery potato scallion desert raisin horseradish spinach carrot soko. Lotus root water spinach fennel kombu maize bamboo shoot green bean swiss chard seakale pumpkin onion chickpea gram corn pea. Brussels sprout coriander water chestnut gourd swiss chard wakame kohlrabi beetroot carrot watercress. Corn amaranth salsify bunya nuts nori azuki bean chickweed potato bell pepper artichoke. </p>
  </div>
</div>
```

**CSS (to complete):**

```css
.container { /* Add styles here */ }
.sidebar { /* Add styles here */ }
```

**Solution:**
This task tests your understanding of `position: fixed`.

```css
.sidebar { 
  position: fixed; 
}
```