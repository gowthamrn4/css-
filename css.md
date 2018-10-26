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
<p>In the following example all <code>&lt;p&gt;</code> elements will be center-aligned, with a red text color:</p>
<p><strong>Example:</strong></p>
<p>p {<br>
color:  red;<br>
text-align:  center;<br>
}</p>
<h2 id="css-selectors">CSS Selectors</h2>
<p>CSS selectors are used to “find” (or select) HTML elements based on their element name, id, class, attribute, and more.</p>
<h2 id="the-element-selector">The element Selector</h2>
<p>The element selector selects elements based on the element name.</p>
<p>You can select all <code>&lt;p&gt;</code> elements on a page like this (in this case, all <code>&lt;p&gt;</code> elements will be center-aligned, with a red text color):<br>
<em><strong>Example:</strong></em></p>
<pre><code>p {  
text-align:  center;  
color:  red;  
}
</code></pre>
<h2 id="the-id-selector">The id Selector</h2>
<p>The id selector uses the id attribute of an HTML element to select a specific element.</p>
<p>The id of an element should be unique within a page, so the id selector is used to select one unique element!</p>
<p>To select an element with a specific id, write a hash (#) character, followed by the id of the element.</p>
<p>The style rule below will be applied to the HTML element with <code>id="para1":</code></p>
<p><em><strong>Example:</strong></em></p>
<pre><code>#para1 {  
text-align:  center;  
color:  red;  
}
</code></pre>
<h2 id="the-class-selector">The class Selector</h2>
<p>The class selector selects elements with a specific class attribute.</p>
<p>To select elements with a specific class, write a period (.) character, followed by the name of the class.</p>
<p>In the example below, all HTML elements with <code>class="center"</code> will be red and center-aligned:<br>
<em><strong>Example:</strong></em></p>
<pre><code>.center {  
text-align:  center;  
color:  red;  
}
</code></pre>
<p>You can also specify that only specific HTML elements should be affected by a class.</p>
<p>In the example below, only <code>&lt;p&gt;</code> elements with <code>class="center"</code> will be center-aligned:</p>
<p><em><strong>Example:</strong></em></p>
<pre><code>p.center {  
text-align:  center;  
color:  red;  
}
</code></pre>
<p>HTML elements can also refer to more than one class.</p>
<p>In the example below, the <code>&lt;p&gt;</code> element will be styled according to <code>class="center"</code> and to <code>class="large":</code></p>
<p><em><strong>Example:</strong></em></p>
<pre><code>p.center {
    text-align: center;
    color: red;
}

p.large {
    font-size: 300%;
}

p .class="center large"
</code></pre>
<h2 id="grouping-selectors">Grouping Selectors</h2>
<p>If you have elements with the same style definitions, like this:</p>
<pre><code>h1 {  
text-align:  center;  
color:  red;  
}  
  
h2 {  
text-align:  center;  
color:  red;  
}  
  
p {  
text-align:  center;  
color:  red;  
}
</code></pre>
<p>(or)</p>
<p>This is grouping selectors</p>
<pre><code>h1, h2, p {  
text-align:  center;            
color:  red;  
}
</code></pre>
<h2 id="css-comments">CSS Comments</h2>
<p>Comments are used to explain the code, and may help when you edit the source code at a later date.</p>
<p>Comments are ignored by browsers.</p>
<p>A CSS comment starts with /* and ends with */. Comments can also span multiple lines:</p>
<pre><code>p {  
color:  red;  
/* This is a single-line comment */  
text-align:  center;  
}  
  
/* This is  
a multi-line  
comment */
</code></pre>
<h2 id="three-ways-to-insert-css">Three Ways to Insert CSS</h2>
<ul>
<li>External style sheet</li>
<li>Internal style sheet</li>
<li>Inline style</li>
</ul>
<h2 id="external-style-sheet">External Style Sheet</h2>
<p>With an external style sheet, you can change the look of an entire website by changing just one file!</p>
<p>Each page must include a reference to the external style sheet file inside the <code>&lt;link&gt;</code> element. The <code>&lt;link&gt;</code> element goes inside the <code>&lt;head&gt;</code> section:</p>
<pre><code>&lt;head&gt;
&lt;link rel="stylesheet" type="text/css" href="mystyle.css"&gt;
&lt;/head&gt;
</code></pre>
<p>Here is how the “mystyle.css” looks:</p>
<pre><code>   body {  
background-color:  lightblue;  
}  
  
h1 {  
color:  navy;  
margin-left:  20px;  
}
</code></pre>
<h2 id="internal-style-sheet">Internal Style Sheet</h2>
<p>An internal style sheet may be used if one single page has a unique style.</p>
<p>Internal styles are defined within the <code>&lt;style&gt;</code> element, inside the <code>&lt;head&gt;</code> section of an HTML page:</p>
<pre><code>   &lt;head&gt;  
        &lt;style&gt;  
        body  {  
        background-color:  linen;  
        }  
          
        h1  {  
        color:  maroon;  
        margin-left:  40px;  
        }  
        &lt;/style&gt;  
        &lt;/head&gt;
</code></pre>
<h2 id="inline-styles">Inline Styles</h2>
<p>An inline style may be used to apply a unique style for a single element.</p>
<p>To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.</p>
<p>The example below shows how to change the color and the left margin of a <code>&lt;h1&gt;</code> element:</p>
<pre><code>&lt;h1 style="color:blue;margin-left:30px;"&gt;This is a heading&lt;/h1&gt;
</code></pre>
<h2 id="multiple-style-sheets">Multiple Style Sheets</h2>
<p>If some properties have been defined for the same selector (element) in different style sheets, the value from the last read style sheet will be used.</p>
<h3 id="example">Example</h3>
<pre><code>&lt;head&gt;  
&lt;link rel="stylesheet"  type="text/css"  href="mystyle.css"&gt;  
&lt;style&gt;  
h1  {  
color:  orange;  
}  
&lt;/style&gt;  
&lt;/head&gt;
</code></pre>
<h2 id="cascading-order">Cascading Order</h2>
<p>What style will be used when there is more than one style specified for an HTML element?</p>
<p>All the styles in a page will “cascade” into a new “virtual” style sheet by the following rules, where number one has the highest priority:</p>
<ul>
<li>
<ol>
<li>Inline style (inside an HTML element)</li>
</ol>
</li>
<li>
<ol start="2">
<li>External and internal style sheets (in the head section)</li>
</ol>
</li>
<li>
<ol start="3">
<li>Browser default</li>
</ol>
</li>
</ul>
<h1 id="css--colors">CSS  Colors</h1>
<p>Colors are specified using predefined color names, or RGB, HEX, HSL, RGBA, HSLA values.</p>
<h2 id="color-names">Color Names</h2>
<p>In HTML, a color can be specified by using a color name:</p>
<p><img src="http://smashinghub.com/wp-content/uploads/2011/11/CSS-Colors1.jpg" alt="enter image description here"></p>

