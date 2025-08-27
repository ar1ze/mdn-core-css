# Web Fonts 📝

In the first article of the module, we explored the basic CSS features available for styling fonts and text. In this article we will go further, exploring web fonts in detail. We'll see how to use custom fonts with your web page to allow for more varied, custom text styling.

-----

## Prerequisites and Objectives 🎯

  * **Prerequisites:** Structuring content with HTML, CSS Styling basics, Fundamental text, and font styling.
  * **Objective:** Understand that web fonts allow developers to go beyond the web-safe font set and use custom fonts on their web apps.
  * Basic setup with the **@font-face** at-rule and common descriptors.
  * Using a web font with the **font-family** property.
  * Using an online service like **Font Squirrel** or **Google Fonts** to find web fonts and generate code.

-----

## Font Families Recap 📜

  * The **font-family** property controls fonts applied to HTML.
  * Browsers find an available font by traveling down a list of font-family values.
  * This system works, but traditionally developers were limited to **"web-safe"** fonts.
  * The **font stack** specifies preferred fonts followed by web-safe alternatives, which can increase workload due to testing.

-----

## What Are Web Fonts? 🌐

  * Web fonts are font files downloaded along with a website.
  * Any browser supporting this CSS feature can display the fonts you've specifically chosen.
  * You use a **@font-face** ruleset at the start of your CSS to specify the font files to download.
  * The syntax:
    ```css
    @font-face {
      font-family: "myFont";
      src: url("myFont.woff2");
    }
    ```
    Then, you apply the font using its family name:
    ```css
    html {
      font-family: "myFont", "Bitstream Vera Serif", serif;
    }
    ```

-----

## Important Considerations for Web Fonts ⚠️

  * **Licensing:** Fonts aren't generally free to use without restrictions. You must pay for them or follow license conditions.
  * **Format Support:** All major browsers support WOFF/WOFF2. WOFF2 supports TrueType and OpenType specifications.
  * **Order of Files:** List your preferred format (WOFF2) first, with older formats afterward, as the browser will choose the first usable file.
  * You can use the **Firefox Font Editor** to inspect and manipulate fonts on a page.

-----

## Adding Your Own Web Fonts 🛠️

1.  **Finding Fonts:** Obtain font files from a free font distributor (like **Font Squirrel**), a paid font distributor, or an online font service. For this example, use Font Squirrel.
2.  **Generating Code:** Use the **Transfonter Webfont Generator** to upload your font files and generate the required WOFF, WOFF2 files, and CSS code.
3.  **Implementing Code:**
      * Rename the unzipped directory to something simple (e.g., `fonts`).
      * Copy the **@font-face** rulesets from the generated `stylesheet.css` into your main CSS file at the very top.
      * Make sure the file paths are correct by adding the directory name, e.g., `fonts/`.
      * Use the font in your font stack as you would any other font.

-----

## Using an Online Font Service ☁️

  * Online services like **Google Fonts** or **Adobe Fonts** store and serve fonts for you, simplifying the process.
  * You typically just need to insert a simple line of HTML code into your `head` section and then use the CSS declarations to apply the font.
  * Google Fonts is a useful free service for rapid testing.

-----

## @font-face in More Detail ⚙️

  * **font-family:** Specifies the name to refer to the font; can be anything you like.
  * **src:** Specifies the paths and formats of the font files. It's best to list your preferred formats first.
  * **font-weight/font-style:** Specify the weight and style of the font. Useful for importing multiple variants of the same font.
  * **font-display:** Specifies how the font is displayed while loading.
  * **unicode-range:** A newer feature that only downloads the font if the page contains the specified characters, saving unnecessary downloads.

-----

## Conclusion 📖

You have now worked through the articles on text styling fundamentals and are ready to test your comprehension with the module challenge: **Typesetting a community school homepage**.