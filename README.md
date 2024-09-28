CSS

Module 1: Introduction to CSS:

**What is CSS?**

CSS stands for Cascading Style Sheets. It\'s a styling language used to
control the layout and appearance of web pages written in HTML or XML.

**Overview of CSS**

CSS is used to separate presentation from structure, making web pages
more visually appealing, user-friendly, and accessible. It allows
developers to:

-   Control typography, colors, and backgrounds

-   Create layouts and positioning

-   Add visual effects and animations

-   Enhance user experience and accessibility

**How CSS works with HTML**

HTML provides the structure, while CSS provides the visual style:

1.  HTML files provide the content and structure.

2.  CSS files provide the layout and visual styling.

3.  Web browsers combine HTML and CSS to render the final web page.

**CSS Syntax**

CSS syntax consists of:

-   **Selectors**: Target HTML elements (.class, #id, tag)

-   **Properties**: Define styles (color, font-size, background-color)

-   **Values**: Assign values to properties (red, 18px, #fff)

Example: h1 { color: blue; font-size: 36px; }

**Inline, Internal, and External CSS**

There are three ways to link CSS to HTML:

1.  **Inline CSS**: Styles applied directly to HTML elements using the
    > style attribute.

   Example: 
>\<h1 style=\"color: blue;\"\>Heading\</h1\>

3.  **Internal CSS**: Styles defined within the HTML document using the
    > \<style\> tag.

    Example:
    > \<style\>h1 { color: blue; }\</style\>

5.  **External CSS**: Styles defined in a separate CSS file linked to
    > the HTML document using the \<link\> tag.

    Example:
    > \<link rel=\"stylesheet\" href=\"styles.css\"\>

**CSS Comments**

CSS comments are used to add notes or explanations:

-   Start with /\*

-   End with \*/

-   Comments are ignored by web browsers

Example: /\* This is a CSS comment \*/

Module 2: Basic Selectors and Properties,

**CSS Selectors**

CSS selectors target HTML elements to apply styles. There are three
basic selectors:

1\. Type Selector (Tag Selector)

Targets elements by their HTML tag name.

Example:

HTML:
> \<p\>This is a paragraph.\</p\>

CSS:
> p { color: blue; }

2\. Class Selector

Targets elements with a specific class attribute.

Example:

HTML:
> \<p class=\"highlight\"\>This is a highlighted paragraph.\</p\>

CSS: 
>.highlight { background-color: yellow; }

3\. ID Selector

Targets a single element with a unique ID attribute.

Example:

HTML: \<p id=\"intro\"\>This is the introduction.\</p\>

CSS: #intro { font-size: 24px; }

**Combining Selectors**

You can combine selectors to target specific elements:

Type and Class

HTML:

\<p class=\"highlight\"\>This is a highlighted paragraph.\</p\>

\<span class=\"highlight\"\>This is highlighted text.\</span\>

CSS:

p.highlight {

background-color: lightblue;

}

**Result**: Only paragraphs with the class \"highlight\" will have a
light blue background.

ID and Class

HTML:

\<p id=\"intro\" class=\"highlight\"\>This is the introduction.\</p\>

CSS:

#intro.highlight {

font-size: 36px;

}

**Result**: Only the paragraph with both ID \"intro\" and class
\"highlight\" will have a font size of 36px.

**Best Practices**

-   Use meaningful class names and IDs.

-   Avoid using generic class names like .red or .big.

-   Use IDs sparingly, as they must be unique.

**Additional Basic Selectors**

-   Universal Selector (\*): Targets all elements.

-   Group Selector (,): Targets multiple elements.

Example

\<h1\>This is a heading.\</h1\>

\<h2\>This is a subheading.\</h2\>

\<p\>This is a paragraph.\</p\>

h1, h2, p {

color: green;

}

Attribute selectors in CSS allow you to target HTML elements based on
their attributes and attribute values. Here\'s a comprehensive overview:

**Attribute Selectors**

1\. \[attribute\]

Targets elements with the specified attribute.

Example:

HTML: \<input type=\"text\" name=\"username\"\>

CSS: input\[type\] { width: 200px; }

2\. \[attribute=\"value\"\]

Targets elements with the specified attribute and exact value.

Example:

HTML: \<input type=\"text\" name=\"username\"\>

CSS: input\[type=\"text\"\] { width: 200px; }

3\. \[attribute\~=\"value\"\]

Targets elements with the specified attribute and value containing the
specified word.

Example:

HTML: \<p class=\"main header\"\>This is a header.\</p\>

CSS: p\[class\~=\"header\"\] { font-size: 24px; }

4\. \[attribute\|=\"value\"\]

Targets elements with the specified attribute and value starting with
the specified string.

Example:

HTML: \<p lang=\"en-US\"\>This is a paragraph.\</p\>

CSS: p\[lang\|=\"en\"\] { font-family: Arial; }

5\. \[attribute\^=\"value\"\]

Targets elements with the specified attribute and value starting with
the specified string.

Example:

HTML: \<img src=\"image1.jpg\"\>

CSS: img\[src\^=\"image\"\] { border: 1px solid black; }

6\. \[attribute\$=\"value\"\]

Targets elements with the specified attribute and value ending with the
specified string.

Example:

HTML: \<img src=\"image1.jpg\"\>

CSS: img\[src\$=\".jpg\"\] { border: 1px solid black; }

7\. \[attribute\*=\"value\"\]

Targets elements with the specified attribute and value containing the
specified string.

Example:

HTML: \<p class=\"main-image\"\>This is a paragraph.\</p\>

CSS: p\[class\*=\"image\"\] { font-size: 18px; }

**Examples and Use Cases**:

-   Form styling: input\[type=\"radio\"\], input\[type=\"checkbox\"\] {
    > /\* styles \*/ }

-   Language-specific styling: p\[lang\|=\"en\"\] { /\* styles \*/ }

-   Image styling: img\[src\$=\".jpg\"\] { /\* styles \*/ }

**Browser Support**:

Attribute selectors are supported in:

-   Chrome 1+

-   Firefox 2+

-   Safari 3+

-   Edge 6+

-   IE 7+ (partial support)

Note: Older browsers may have partial or no support for attribute
selectors.
