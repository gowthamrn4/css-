---


---

<ol>
<li>Content:</li>
</ol>
<ul>
<li>CSS Syntax</li>
<li></li>
</ul>
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
<h2 id="background-color">Background Color</h2>
<p>You can set the background color for HTML elements:<br>
<strong>Example:</strong></p>
<pre><code>&lt;h1 style="background-color:DodgerBlue;"&gt;Hello World&lt;/h1&gt;  
&lt;p style="background-color:Tomato;"&gt;Lorem ipsum...&lt;/p&gt;
</code></pre>
<p><img src="https://css-tricks.com/wp-content/uploads/2011/05/fullwidthbars.png" alt="enter image description here"></p>
<h2 id="text-color">Text Color</h2>
<p>You can set the color of text:</p>
<pre><code>&lt;h1 style="color:Tomato;"&gt;Hello World&lt;/h1&gt;  
&lt;p style="color:DodgerBlue;"&gt;Lorem ipsum...&lt;/p&gt;  
&lt;p style="color:MediumSeaGreen;"&gt;Ut wisi enim...&lt;/p&gt;
</code></pre>
<p><img src="https://stuyhsdesign.files.wordpress.com/2015/09/external-style.png" alt="enter image description here"></p>
<h2 id="border-color">Border Color</h2>
<p>You can set the color of borders:</p>
<pre><code>&lt;h1 style="border:2px solid Tomato;"&gt;Hello World&lt;/h1&gt;  
&lt;h1 style="border:2px solid DodgerBlue;"&gt;Hello World&lt;/h1&gt;  
&lt;h1 style="border:2px solid Violet;"&gt;Hello World&lt;/h1&gt;
</code></pre>
<p><img src="data:image/png;base64,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" alt="enter image description here"></p>
<h2 id="color-values">Color Values</h2>
<p>In HTML, colors can also be specified using RGB values, HEX values, HSL values, RGBA values, and HSLA values:</p>
<p>Same as color name “Tomato”:</p>
<pre><code>&lt;h1 style="background-color:rgb(255, 99, 71);"&gt;...&lt;/h1&gt;  
&lt;h1 style="background-color:#ff6347;"&gt;...&lt;/h1&gt;  
&lt;h1 style="background-color:hsl(9, 100%, 64%);"&gt;...&lt;/h1&gt;  
  
&lt;h1 style="background-color:rgba(255, 99, 71, 0.5);"&gt;...&lt;/h1&gt;  
&lt;h1 style="background-color:hsla(9, 100%, 64%, 0.5);"&gt;...&lt;/h1&gt;
</code></pre>
<p><img src="https://2.bp.blogspot.com/-QHbaSem0PSs/W2k7OpPlEzI/AAAAAAAAATc/ZOW7tGgh3Kkd7u6B2DhI1IG0TFj3CnHoACLcBGAs/s640/HTML+color.PNG" alt="enter image description here"></p>
<h1 id="css--backgrounds">CSS  Backgrounds</h1>
<p>The CSS background properties are used to define the background effects for elements.</p>
<p>CSS background properties:</p>
<ul>
<li>background-color</li>
<li>background-image</li>
<li>background-repeat</li>
<li>background-attachment</li>
<li>background-position</li>
</ul>
<h2 id="background-color-1">Background Color</h2>
<p>The  <code>background-color</code>  property specifies the background color of an element.</p>
<p>The background color of a page is set like this:</p>
<pre><code>body {  
background-color:  lightblue;  
}
</code></pre>
<p>With CSS, a color is most often specified by:</p>
<ul>
<li>a valid color name - like “red”</li>
<li>a HEX value - like “#ff0000”</li>
<li>an RGB value - like “rgb(255,0,0)”</li>
</ul>
<p>Example:</p>
<pre><code>h1 {  
background-color:  green;  
}  
  
div {  
background-color:  lightblue;  
}  
  
p {  
background-color:  yellow;  
}
</code></pre>
<h2 id="background-image">Background Image</h2>
<p>The  <code>background-image</code>  property specifies an image to use as the background of an element.</p>
<p>By default, the image is repeated so it covers the entire element.</p>
<p>The background image for a page can be set like this:</p>
<pre><code>body {  
background-image:  url("paper.gif");  
}
</code></pre>
<p>Below is an example of a <strong>bad</strong> combination of text and background image. The text is hardly readable:</p>
<pre><code>body {  
background-image:  url("bgdesert.jpg");  
}
</code></pre>
<h2 id="background-image---repeat-horizontally-or-vertically">Background Image - Repeat Horizontally or Vertically</h2>
<p>By default, the  <code>background-image</code>  property repeats an image both horizontally and vertically.</p>
<p>Some images should be repeated only horizontally or vertically, or they will look strange, like this:</p>
<pre><code>body {  
background-image:  url("gradient_bg.png");  
}
</code></pre>

