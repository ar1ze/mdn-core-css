# CSS Media Queries 💻
---
The CSS Media Query allows you to apply CSS based on the browser and device environment, a key part of responsive web design.


### Learning Outcomes 🧠
* Syntax of media queries
* Common media query types
* Using width and height queries for responsive layouts
* Choosing breakpoints
* Implementing a mobile-first design

## Media Query Basics 📜
---
A simple media query looks like this:

`@media media-type and (media-feature-rule) { /* CSS rules */ }`

* **Media Type**: Specifies the kind of media (e.g., `print` or `screen`).
* **Media Expression**: A rule or test that must pass for the CSS to apply.
* **CSS Rules**: The styles to be applied if the test passes.

### Media Types 📄
* `all`
* `print`
* `screen`

**Note**: Media types are optional. If omitted, the query defaults to `all`.

### Media Feature Rules 📏
* **`width` and `height`**: Detect viewport dimensions. Can be prefixed with `min-` or `max-`.
    * `@media screen and (max-width: 600px)`: Applies styles if the viewport is 600px or narrower.
* **`orientation`**: Tests for `portrait` or `landscape` orientation.
* **`hover`**: Tests if the user can hover over an element (e.g., using a mouse).
* **`pointer`**: Detects the type of pointing device (`none`, `fine`, or `coarse`).

### Ranged Syntax ➡️
A more readable way to specify a range:
`@media (30em <= width <= 50em)`

## More Complex Media Queries 🔗
---
* **`and` logic**: Combine multiple features.
    * `@media screen and (width >= 600px) and (orientation: landscape)`
* **`or` logic**: Comma-separate queries.
    * `@media screen and (width >= 600px), screen and (orientation: landscape)`
* **`not` logic**: Negates the entire query.
    * `@media not (width >= 600px)`

## Choosing Breakpoints 🎯
---
* **Avoid targeting specific devices.**
* Choose breakpoints where the content starts to break or become unreadable.
* Use browser developer tools (e.g., Firefox Responsive Design Mode) to find optimal breakpoints.

## Mobile-First Responsive Design 📱
---
* Start with the smallest view and add layout adjustments as the viewport gets larger.
* This approach is often the best because a single-column layout for small screens is the default.

### `viewport` meta tag 🌐
` <meta name="viewport" content="width=device-width,initial-scale=1" /> `
* This tag ensures mobile browsers render content using the device's real width, not a fixed viewport.

## Do You Really Need a Media Query? 🤔
---
* Modern CSS layout methods like **Flexbox** and **CSS Grid** can create flexible, responsive components without media queries.
* It is always worth considering if these methods alone can solve the layout problem.
* Best results often come from using a combination of modern layout methods and media queries.

## Summary 📝
---
* Media queries are a powerful tool for responsive design.
* Experiment with different queries and layout methods to find the best solution for your content.
* The next article will provide tests to check your understanding.