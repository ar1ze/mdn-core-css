# Combinators

---

The final selectors we will look at are called **combinators**. Combinators are used to combine other selectors in a way that allows us to select elements based on their location in the **DOM** relative to other elements (for example, child or sibling).

### Prerequisites
* **HTML basics** (study Basic HTML syntax)
* **Basic CSS selectors**

### Learning Outcomes
* The basic concept of combinators.
* Descendant and child combinators.
* Next- and subsequent-sibling combinators.
* Nesting.
* Combining combinators with selectors.

---

### 1. Descendant Combinator ( ) 👨‍👧‍👦

* Represented by a **single space** character.
* Combines two selectors to select an element if it has an **ancestor** (parent, grandparent, etc.) matching the first selector.
* Example: `css .box p { color: red; }` matches a `<p>` element inside an element with a class of `.box`.

---

### 2. Child Combinator (>) 👶

* Placed between two CSS selectors.
* Matches only those elements that are the **direct children** of elements matched by the first selector.
* Example: `css article > p { /* ... */ }` selects only `<p>` elements that are direct children of `<article>` elements.

---

### 3. Next-Sibling Combinator (+) ➡️

* Placed between two CSS selectors.
* Matches only those elements that **come immediately after** the element matched by the first selector.
* Example: `css h1 + p { /* ... */ }` selects any paragraph that immediately follows an `<h1>`.

---

### 4. Subsequent-Sibling Combinator (~) 〰️

* Used to select siblings of an element even if they are **not directly adjacent**.
* Matches all elements that come **anywhere after** the first selector within the same parent.
* Example: `css h1 ~ p { /* ... */ }` selects all `<p>` elements that come after the `<h1>`.

---

### 5. Combining Combinators with Selectors 🧪

* You can combine any of the selectors (e.g., class, attribute) with combinators.
* Example: `css ul > li[class="a"] { }` selects list items with a class of `a` which are direct children of a `<ul>`.
* **Caution**: Creating overly specific selectors can make your CSS hard to reuse. It is often better to use a simple class.