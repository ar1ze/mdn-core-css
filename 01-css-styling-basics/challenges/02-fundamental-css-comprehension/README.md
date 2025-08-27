# Challenge: Fundamental CSS Comprehension 🚀

---

This challenge provides a series of exercises to create a business card, gamer card, or social media profile using CSS.

## 🎯 Project Brief

You'll be provided with raw HTML and an image and tasked with writing the necessary CSS to style them into a "nifty little online business card."

### **Basic Setup** 🛠️
* Create a new file named `style.css` in the same directory as your HTML and image files.
* Link the CSS file to your HTML using a `<link>` element.
* Copy and paste the first two rulesets from the provided CSS resource file into the top of your new file.
* Add a CSS comment at the top for "General page styles."
* Add three more comments at the bottom for card container styles, header/footer styles, and main content styles.

### **Working with Provided Selectors** ✍️
* Calculate the specificity for the four selectors in the CSS resource file and write them down in a comment.
* Match the correct selectors to their rulesets to:
    * Give the main card container a fixed width/height, background color, border, and `border-radius`.
    * Give the header and footer background gradients and rounded corners that match the container.
    * Float the image to the right with a `max-height` of 100%.
* Fix the two errors in the provided rulesets.

### **Writing New Rulesets** 📝
* Target both the card header and footer and give them a total height of **50px** (content height 30px + 10px padding on all sides) expressed in `ems`.
* Set the margin to `0` for all `<h2>` and `<p>` elements.
* Set the `<article>` height to **120px** in `ems` and give it a semi-transparent black background.
* Set the `<h2>` font size to **20px** in `ems` with a line height to center it in the header's content box.
* Set the `<p>` inside the footer to a font size of **15px** in `ems` with a line height to center it in the footer's content box.
* Add padding to the paragraph inside the `<article>` so it lines up with the `<h2>` and footer `<p>`, and set its color to a light value for readability.

### **Important Notes** 💡
* The second ruleset sets `font-size: 10px;` on the `<html>` element, making `1em` equal to `10px` for its descendants.
* Use separate declarations on each line for maximum readability.
* Start all your rules with `.card` to avoid styling conflicts.

## 💡 Hints and Tips

---

* You don't need to edit the HTML, only link to the CSS.
* To calculate the `em` value, think about what the root font size needs to be multiplied by to get the desired pixel length.