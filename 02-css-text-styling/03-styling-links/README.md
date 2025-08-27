# 🔗 Styling Links

This article explains how to style links in CSS, focusing on why default styles are important and how to use pseudo-classes to create effective and accessible link designs.

-----

## Prerequisites & Learning Outcomes

### Prerequisites

  * **Structuring content with HTML**
  * **CSS Styling basics**

### Learning Outcomes

  * Understand the importance of **default link styles** for usability.
  * Master styling different **link states** using pseudo-classes.
  * Learn how to include **icons on links**.
  * Create a **navigation menu** with links.

-----

## 🚦 Link States

Links can exist in different states, which you can style using specific pseudo-classes:

  * `:link`: An unvisited link.
  * `:visited`: A link that a user has already visited.
  * `:hover`: When the user's mouse pointer is over the link.
  * `:focus`: When the link is selected, e.g., by a keyboard user using the Tab key.
  * `:active`: When the link is being clicked or activated.  

  This order is important because link styles build on one another. For example, the styles in the first rule will apply to all the subsequent ones. When a link is activated, it's usually also hovered over. If you put these in the wrong order, and you're changing the same properties in each ruleset, things won't work as you expect. To remember the order, you could try using a mnemonic like LoVe Fears HAte.

-----

## 🎨 Default Styles & Best Practices

Default link styles have been around since the 1990s because users expect them. It's crucial not to stray too far from these conventions to maintain usability.

### Default Properties:

  * **Underlined**
  * **Blue** (unvisited) or **purple** (visited) text color.
  * Mouse pointer changes to a **hand icon** on hover.
  * A **focus outline** appears when tabbed to.
  * **Red** text when active.

### Recommended Practices:

  * Always use underlining for links, but not for other text.
  * If not underlining, highlight links in some other clear way.
  * Ensure links react to `:hover`, `:focus`, and `:active` states.
  * The default focus outline is an accessibility aid and should only be removed if you provide another clear visual indicator.

-----

## ✨ Styling Links with CSS

The order of pseudo-classes matters. A useful mnemonic is **LoVe Fears HAte** to remember the correct order: `:link`, `:visited`, `:focus`, `:hover`, `:active`.

### Example CSS:

```css
a {
  outline-color: transparent;
}
a:link {
  color: #6900ff;
}
a:visited {
  color: #a5c300;
}
a:focus {
  text-decoration: none;
  background: #bae498;
}
a:hover {
  text-decoration: none;
  background: #cdfeaa;
}
a:active {
  background: #6900ff;
  color: #cdfeaa;
}
```

-----

## 🖼️ Including Icons on Links

You can use the `::after` pseudo-element to add icons to links, such as an external link icon.

### CSS Example:

```css
a[href^="http"]::after {
  content: "";
  display: inline-block;
  width: 0.8em;
  height: 0.8em;
  margin-left: 0.25em;
  background-size: 100%;
  background-image: url("external-link-52.png");
}
```

  * The `a[href^="http"]` attribute selector targets links whose `href` attribute starts with "http," effectively selecting external links.

-----

## 🔘 Styling Links as Buttons

Links are often styled to look like buttons or tabs, particularly in navigation menus.

### HTML & CSS Example:

```html
<nav class="container">
  <a href="#">Home</a>
  <a href="#">Pizza</a>
</nav>
```

```css
.container {
  display: flex;
  gap: 0.625%;
}
a {
  flex: 1;
  text-decoration: none;
  outline-color: transparent;
  text-align: center;
  line-height: 3;
  color: black;
}
a:link, a:visited, a:focus {
  background: palegoldenrod;
  color: black;
}
a:hover {
  background: orange;
}
a:active {
  background: darkred;
  color: white;
}
```