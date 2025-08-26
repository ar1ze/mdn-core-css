# Test your skills: Sizing 📏

-----

The aim of this skill test is to help you assess whether you understand the different ways of sizing items in CSS.

-----

## Task 1 📦

In this task, you have two boxes. To complete the task:

  - **Size the first box** so that the height will be at least **100px**, but the content should not overflow if there is more content than fits.
  - **Size the second box** so that it is fixed at **100px** tall, so that content will overflow if there is too much.

### HTML

```html
<div class="box box1">
  <p>
    Veggies es bonus vobis, proinde vos postulo essum magis kohlrabi welsh onion
    daikon amaranth tatsoi tomatillo melon azuki bean garlic. Gumbo beet greens
    corn soko endive gumbo gourd.
  </p>
</div>

<div class="box box2">
  <p>
    Veggies es bonus vobis, proinde vos postulo essum magis kohlrabi welsh onion
    daikon amaranth tatsoi tomatillo melon azuki bean garlic. Gumbo beet greens
    corn soko endive gumbo gourd.
  </p>
</div>
```

### CSS

```css
.box1 {
  min-height: 100px;
}

.box2 {
  height: 100px;
}
```

-----

## Task 2 🖼️

In this task, you have a box, which contains another box. To complete the task:

  - Make the inner box width **60%** of the width of the outer box.
  - Give the inner box padding of **10%** using the width as the size from which that percentage is calculated.

### HTML

```html
<div class="box">
  <div class="inner">Make me 60% of my parent's width.</div>
</div>
```

### CSS

```css
* {
  box-sizing: border-box;
}
.inner {
  width: 60%;
  padding: 10%;
}
```

-----

## Task 3 🏞️

In this task, you have two images in boxes. To complete the task, apply a declaration to the image so that:

  - The large image shrinks down into the box.
  - The small image does not stretch.

### HTML

```html
<div class="box">
  <img
    alt="A pink star"
    src="https://mdn.github.io/shared-assets/images/examples/star-pink_256x256.png"
  />
</div>

<div class="box">
  <img
    alt="Hot air balloons flying in clear sky, and a crowd of people in the foreground"
    src="https://mdn.github.io/shared-assets/images/examples/balloons.jpg"
  />
</div>
```

### CSS

```css
img {
  max-width: 100%;
}
```