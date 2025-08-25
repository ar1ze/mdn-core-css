# 📝 CSS Attribute Selectors

---

### Introduction
* As you know from your study of HTML, elements can have **attributes** that give further detail about the element being marked up.
* In CSS, you can use **attribute selectors** to target elements with certain attributes.
* This lesson shows you how to use these useful selectors.

### Prerequisites
* HTML basics
* Basic CSS selectors

### Learning Outcomes
* The basic concept of attribute selectors.
* Presence and value attribute selectors.
* Substring matching attribute selectors.

---

### Presence and Value Selectors

These selectors select an element based on the **presence of an attribute alone** or on **different matches against the attribute's value**.

| Selector | Example | Description |
| :--- | :--- | :--- |
| `[attr]` | `a[title]` | Matches elements with a specified attribute. |
| `[attr=value]` | `a[href="https://example.com"]` | Matches elements with an attribute whose value is **exactly** the string inside the quotes. |
| `[attr~=value]` | `p[class~="special"]` | Matches elements with an attribute whose value is a **space-separated list** containing the exact value. |
| `[attr|=value]` | `div[lang\|="zh"]` | Matches elements with an attribute whose value is **exactly** the specified value or begins with the value immediately followed by a hyphen. |

---

### Substring Matching Selectors

These selectors allow for more **advanced matching of substrings** inside the value of your attribute.

| Selector | Example | Description |
| :--- | :--- | :--- |
| `[attr^=value]` | `li[class^="box-"]` | Matches elements with an attribute whose value **begins with** the specified string. |
| `[attr$=value]` | `li[class$="-box"]` | Matches elements with an attribute whose value **ends with** the specified string. |
| `[attr*=value]` | `li[class*="box"]` | Matches elements with an attribute whose value **contains** the specified string anywhere. |

---

### Summary
* Attribute selectors are a powerful way to target HTML elements for styling.
* This lesson covered **presence and value selectors** as well as **substring matching selectors**.
* The next article will cover **pseudo-class** and **pseudo-element selectors**.