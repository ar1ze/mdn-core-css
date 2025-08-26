
# Handling CSS Conflicts 📝

---

### Key Concepts

* **Cascade**: The rules that determine how CSS is applied and how conflicts are resolved. The order and origin of your CSS rules matter. 
* **Specificity**: An algorithm the browser uses to decide which rule applies when multiple rules target the same element. It's a measure of how specific a selector is.
* **Inheritance**: The way some CSS properties pass their values down from a parent element to its children.

### The Cascade in Detail 🌊

* When rules have the same specificity, the one that appears last in the stylesheet wins.
* **Specificity** determines which rule wins when selectors are different. A selector with higher specificity will always override one with lower specificity, regardless of its position in the stylesheet.
    * **ID Selector**: Highest specificity.
    * **Class, Attribute, Pseudo-class Selectors**: Medium specificity.
    * **Element, Pseudo-element Selectors**: Lowest specificity.
    * **Calculation**: Specificity is measured by counting IDs, classes, and elements (e.g., `#header .nav-item` would be 1-1-0).
* **`!important`**: This flag overrides all other rules, including inline styles. It should be used with extreme caution as it makes debugging difficult.

---

### Inheritance in Detail 🏡

* Some properties, like `color` and `font-family`, are inherited by default.
* Some properties, like `width`, `margin`, and `border`, are not inherited.
* **Universal Property Values**:
    * `inherit`: Forces a property to take its value from the parent.
    * `initial`: Resets a property to its browser default value.
    * `revert`: Resets the property to the browser's default styling.
    * `unset`: Behaves like `inherit` for naturally inherited properties and `initial` for non-inherited properties.
    * `all`: A shorthand property that can apply `initial`, `inherit`, or `unset` to all properties at once.

---

### Order of Overriding Declarations ⚖️

Declarations are applied in this order, with later ones overriding earlier ones:

1.  User agent style sheets (browser defaults)
2.  Normal declarations in user style sheets (user's custom styles)
3.  Normal declarations in author style sheets (developer's styles)
4.  `!important` declarations in author style sheets
5.  `!important` declarations in user style sheets
6.  `!important` declarations in user agent style sheets