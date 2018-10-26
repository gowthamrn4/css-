---


---

<h1 id="css--introduction">CSS  Introduction</h1>
<h2 id="what-is-css">What is css?</h2>
<ul>
<li><strong>CSS</strong>  stands for  <strong>C</strong>ascading  <strong>S</strong>tyle  <strong>S</strong>heets</li>
<li>CSS describes  <strong>how HTML elements are to be displayed on screen, paper, or in other media</strong></li>
<li>CSS  <strong>saves a lot of work</strong>. It can control the layout of multiple web pages all at once</li>
<li>External stylesheets are stored in  <strong>CSS files</strong></li>
</ul>
<h2 id="why-use-css">Why Use Css?</h2>
<p>CSS is used to define styles for your web pages, including the design, layout and variations in display for different devices and screen sizes.</p>
<h2 id="css-syntax">CSS Syntax</h2>
<p>A CSS rule-set consists of a selector and a declaration block:<br>
The selector points to the HTML element you want to style.</p>
<p>The declaration block contains one or more declarations separated by semicolons.</p>
<p>Each declaration includes a CSS property name and a value, separated by a colon.</p>
<p>A CSS declaration always ends with a semicolon, and declaration blocks are surrounded by curly braces.</p>
<p>In the following example all </p><p> elements will be center-aligned, with a red text color:</p>
<p><strong>Example:</strong><br>
p {<br>
color:  red;<br>
text-align:  center;<br>
}</p>
<h2 id="css-selectors">CSS Selectors</h2>
<p>CSS selectors are used to “find” (or select) HTML elements based on their element name, id, class, attribute, and more.</p>
<h2 id="the-element-selector">The element Selector</h2>
<p>The element selector selects elements based on the element name.</p>
<p>You can select all </p><p> elements on a page like this (in this case, all </p><p> elements will be center-aligned, with a red text color):<br>
<em><strong>Example:</strong></em><br>
p {<br>
text-align:  center;<br>
color:  red;<br>
}</p>
<h2 id="the-id-selector">The id Selector</h2>
<p>The id selector uses the id attribute of an HTML element to select a specific element.</p>
<p>The id of an element should be unique within a page, so the id selector is used to select one unique element!</p>
<p>To select an element with a specific id, write a hash (#) character, followed by the id of the element.</p>
<p>The style rule below will be applied to the HTML element with id=“para1”:</p>
<p><em><strong>Example:</strong></em></p>
<p>#para1 {<br>
text-align:  center;<br>
color:  red;<br>
}</p>
<h2 id="the-class-selector">The class Selector</h2>
<p>The class selector selects elements with a specific class attribute.</p>
<p>To select elements with a specific class, write a period (.) character, followed by the name of the class.</p>
<p>In the example below, all HTML elements with class=“center” will be red and center-aligned:<br>
<em><strong>Example:</strong></em></p>
<p>.center {<br>
text-align:  center;<br>
color:  red;<br>
}</p>
<p>You can also specify that only specific HTML elements should be affected by a class.</p>
<p>In the example below, only </p><p> elements with class=“center” will be center-aligned:</p>
<p><em><strong>Example:</strong></em></p>
<p>p.center {<br>
text-align:  center;<br>
color:  red;<br>
}</p>

