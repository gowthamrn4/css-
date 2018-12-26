---


---

<ol>
<li>Content:</li>
</ol>
<ul>
<li>CSS Syntax</li>
<li>How to Use Css Extr</li>
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
<h1 id="css--borders">CSS  Borders</h1>
<p>The CSS <code>border</code> properties allow you to specify the style, width, and color of an element’s border.</p>
<h2 id="border-style">Border Style</h2>
<ul>
<li><code>dotted</code>  - Defines a dotted border</li>
<li><code>dashed</code>  - Defines a dashed border</li>
<li><code>solid</code>  - Defines a solid border</li>
<li><code>double</code>  - Defines a double border</li>
<li><code>groove</code>  - Defines a 3D grooved border. The effect depends on the border-color value</li>
<li><code>ridge</code>  - Defines a 3D ridged border. The effect depends on the border-color value</li>
<li><code>inset</code>  - Defines a 3D inset border. The effect depends on the border-color value</li>
<li><code>outset</code>  - Defines a 3D outset border. The effect depends on the border-color value</li>
<li><code>none</code>  - Defines no border</li>
<li><code>hidden</code>  - Defines a hidden border</li>
<li>
<h2 id="border-width">Border Width</h2>
</li>
</ul>
<p>The  <code>border-width</code>  property specifies the width of the four borders.</p>
<p>The width can be set as a specific size (in px, pt, cm, em, etc) or by using one of the three pre-defined values: thin, medium, or thick.</p>
<p>The  <code>border-width</code>  property can have from one to four values (for the top border, right border, bottom border, and the left border).</p>
<pre><code>p.one {  
border-style:  solid;  
border-width:  5px;  
}  
  
p.two {  
border-style:  solid;  
border-width:  medium;  
}  
  
p.three {  
border-style:  solid;  
border-width:  2px 10px 4px 20px;  
}
</code></pre>
<h2 id="border-color-1">Border Color</h2>
<p>The  <code>border-color</code>  property is used to set the color of the four borders.</p>
<p>The color can be set by:</p>
<ul>
<li>name - specify a color name, like “red”</li>
<li>Hex - specify a hex value, like “#ff0000”</li>
<li>RGB - specify a RGB value, like “rgb(255,0,0)”</li>
<li>transparent</li>
</ul>
<h2 id="border---shorthand-property">Border - Shorthand Property</h2>
<p>As you can see from the examples above, there are many properties to consider when dealing with borders.</p>
<p>To shorten the code, it is also possible to specify all the individual border properties in one property.</p>
<p>The  <code>border</code>  property is a shorthand property for the following individual border properties:</p>
<ul>
<li>
<p><code>border-width</code></p>
</li>
<li>
<p><code>border-style</code>  (required)</p>
</li>
<li>
<p><code>border-color</code></p>
<p>p {<br>
border:  5px solid red;<br>
}</p>
</li>
</ul>
<h2 id="css-margins">CSS Margins</h2>
<p>The CSS  <code>margin</code>  properties are used to create space around elements, outside of any defined borders.</p>
<p>With CSS, you have full control over the margins. There are properties for setting the margin for each side of an element (top, right, bottom, and left).</p>
<ul>
<li>
<p><code>margin-top</code></p>
</li>
<li>
<p><code>margin-right</code></p>
</li>
<li>
<p><code>margin-bottom</code></p>
</li>
<li>
<p><code>margin-left</code></p>
</li>
<li>
<p>All the margin properties can have the following values:</p>
</li>
<li>
<p>auto - the browser calculates the margin</p>
</li>
<li>
<p><em>length</em>  - specifies a margin in px, pt, cm, etc.</p>
</li>
<li>
<p><em>%</em>  - specifies a margin in % of the width of the containing element</p>
</li>
<li>
<p>inherit - specifies that the margin should be inherited from the parent element</p>
</li>
</ul>
<p><strong>Tip:</strong>  Negative values are allowed.</p>
<h2 id="margin---shorthand-property">Margin - Shorthand Property</h2>
<ul>
<li><code>margin-top</code></li>
<li><code>margin-right</code></li>
<li><code>margin-bottom</code></li>
<li><code>margin-left</code></li>
</ul>
<p><strong>margin: 25px 50px 75px 100px;</strong></p>
<ul>
<li>top margin is 25px</li>
<li>right margin is 50px</li>
<li>bottom margin is 75px</li>
<li>left margin is 100px</li>
</ul>
<h1 id="css--padding">CSS  Padding</h1>
<p>The CSS <code>padding</code> properties are used to generate space around an element’s content, inside of any defined borders.</p>
<ul>
<li>
<p><code>padding-top</code></p>
</li>
<li>
<p><code>padding-right</code></p>
</li>
<li>
<p><code>padding-bottom</code></p>
</li>
<li>
<p><code>padding-left</code></p>
</li>
<li>
<p>All the padding properties can have the following values:</p>
</li>
<li>
<p><em>length</em>  - specifies a padding in px, pt, cm, etc.</p>
</li>
<li>
<p><em>%</em>  - specifies a padding in % of the width of the containing element</p>
</li>
<li>
<p>inherit - specifies that the padding should be inherited from the parent element</p>
</li>
</ul>
<p><strong>Note:</strong>  Negative values are not allowed.</p>
<h2 id="padding---shorthand-property">Padding - Shorthand Property</h2>
<ul>
<li><code>padding-top</code></li>
<li><code>padding-right</code></li>
<li><code>padding-bottom</code></li>
<li><code>padding-left</code></li>
</ul>
<p>So, here is how it works:</p>
<p>If the  <code>padding</code>  property has four values:</p>
<ul>
<li><strong>padding: 25px 50px 75px 100px;</strong>
<ul>
<li>top padding is 25px</li>
<li>right padding is 50px</li>
<li>bottom padding is 75px</li>
<li>left padding is 100px</li>
</ul>
</li>
</ul>
<h1 id="css--height-and-width">CSS  Height and Width</h1>
<p>The  <code>height</code>  and  <code>width</code>  properties are used to set the height and width of an element.</p>
<p>The  <code>height</code>  and  <code>width</code>  can be set to auto (this is default. Means that the browser calculates the height and width), or be specified in  <em>length values</em>, like px, cm, etc., or in percent (%) of the containing block.</p>
<pre><code>div {  
height:  200px;  
width:  50%;  
background-color:  powderblue;  
}
</code></pre>
<h2 id="setting-max-width">Setting max-width</h2>
<p>The  <code>max-width</code>  property is used to set the maximum width of an element.</p>
<p>The  <code>max-width</code>  can be specified in  <em>length values</em>, like px, cm, etc., or in percent (%) of the containing block, or set to none (this is default. Means that there is no maximum width).</p>
<pre><code>div {  
max-width:  500px;  
height:  100px;  
background-color:  powderblue;  
}
</code></pre>
<h1 id="css--box-model">CSS  Box Model</h1>
<p>All HTML elements can be considered as boxes. In CSS, the term “box model” is used when talking about design and layout.</p>
<p>The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content. The image below illustrates the box model:</p>
<ul>
<li>
<p><strong>Content</strong>  - The content of the box, where text and images appear</p>
</li>
<li>
<p><strong>Padding</strong>  - Clears an area around the content. The padding is transparent</p>
</li>
<li>
<p><strong>Border</strong>  - A border that goes around the padding and content</p>
</li>
<li>
<p><strong>Margin</strong>  - Clears an area outside the border. The margin is transparent</p>
<p>div {<br>
width:  300px;<br>
border:  25px solid green;<br>
padding:  25px;<br>
margin:  25px;<br>
}</p>
<h1 id="css--outline">CSS  Outline</h1>
<p>An outline is a line that is drawn around elements, OUTSIDE the borders, to make the element “stand out”.</p>
</li>
<li>
<p><code>outline-style</code></p>
</li>
<li>
<p><code>outline-color</code></p>
</li>
<li>
<p><code>outline-width</code></p>
</li>
<li>
<p><code>outline-offset</code></p>
</li>
<li>
<p><code>outline</code></p>
</li>
</ul>
<h2 id="outline-style">Outline Style</h2>
<ul>
<li>
<p><code>dotted</code>  - Defines a dotted outline</p>
</li>
<li>
<p><code>dashed</code>  - Defines a dashed outline</p>
</li>
<li>
<p><code>solid</code>  - Defines a solid outline</p>
</li>
<li>
<p><code>double</code>  - Defines a double outline</p>
</li>
<li>
<p><code>groove</code>  - Defines a 3D grooved outline</p>
</li>
<li>
<p><code>ridge</code>  - Defines a 3D ridged outline</p>
</li>
<li>
<p><code>inset</code>  - Defines a 3D inset outline</p>
</li>
<li>
<p><code>outset</code>  - Defines a 3D outset outline</p>
</li>
<li>
<p><code>none</code>  - Defines no outline</p>
</li>
<li>
<p><code>hidden</code>  - Defines a hidden outline</p>
<p>p.dotted {outline-style:  dotted;}<br>
p.dashed {outline-style:  dashed;}<br>
p.solid {outline-style:  solid;}<br>
p.double {outline-style:  double;}<br>
p.groove {outline-style:  groove;}<br>
p.ridge {outline-style:  ridge;}<br>
p.inset {outline-style:  inset;}<br>
p.outset {outline-style:  outset;}</p>
</li>
</ul>
<h2 id="outline-color">Outline Color</h2>
<p>The  <code>outline-color</code>  property is used to set the color of the outline.</p>
<ul>
<li>name - specify a color name, like “red”</li>
<li>RGB - specify a RGB value, like “rgb(255,0,0)”</li>
<li>Hex - specify a hex value, like “#ff0000”</li>
<li>invert - performs a color inversion (which ensures that the outline is visible, regardless of color background)</li>
</ul>
<h2 id="outline-width">Outline Width</h2>
<p>The <code>outline-width</code> property specifies the width of the outline, and can have one of the following values:</p>
<ul>
<li>thin (typically 1px)</li>
<li>medium (typically 3px)</li>
<li>thick (typically 5px)</li>
<li>A specific size (in px, pt, cm, em, etc)</li>
</ul>
<h1 id="css--text">CSS  Text</h1>
<p>The  <code>color</code>  property is used to set the color of the text. The color is specified by:</p>
<ul>
<li>
<p>a color name - like “red”</p>
</li>
<li>
<p>a HEX value - like “#ff0000”</p>
</li>
<li>
<p>an RGB value - like “rgb(255,0,0)”</p>
<ul>
<li>body {<br>
color:  blue;<br>
}</li>
</ul>
<p>h1 {<br>
color:  green;<br>
}</p>
</li>
</ul>
<h2 id="text-alignment">Text Alignment</h2>
<p>The  <code>text-align</code>  property is used to set the horizontal alignment of a text.</p>
<p>A text can be left or right aligned, centered, or justified.</p>
<pre><code>h1 {  
text-align:  center;  
}  
  
h2 {  
text-align:  left;  
}  
  
h3 {  
text-align:  right;  
}
</code></pre>
<h2 id="text-decoration">Text Decoration</h2>
<p>The  <code>text-decoration</code>  property is used to set or remove decorations from text.</p>
<p>The value  <code>text-decoration: none;</code>  is often used to remove underlines from links:</p>
<pre><code>a {  
text-decoration:  none;  
}
</code></pre>
<h2 id="text-transformation">Text Transformation</h2>
<p>The  <code>text-transform</code>  property is used to specify uppercase and lowercase letters in a text.</p>
<p>It can be used to turn everything into uppercase or lowercase letters, or capitalize the first letter of each word:</p>
<pre><code>p.uppercase {  
text-transform:  uppercase;  
}  
  
p.lowercase {  
text-transform:  lowercase;  
}  
  
p.capitalize {  
text-transform:  capitalize;  
}
</code></pre>
<h2 id="text-indentation">Text Indentation</h2>
<p>The  <code>text-indent</code>  property is used to specify the indentation of the first line of a text:</p>
<pre><code>p {  
text-indent:  50px;  
}
</code></pre>
<h2 id="letter-spacing">Letter Spacing</h2>
<p>The  <code>letter-spacing</code>  property is used to specify the space between the characters in a text.</p>
<p>The following example demonstrates how to increase or decrease the space between characters:</p>
<pre><code>h1 {  
letter-spacing:  3px;  
}  
  
h2 {  
letter-spacing:  -3px;  
}
</code></pre>
<h2 id="line-height">Line Height</h2>
<p>The  <code>line-height</code>  property is used to specify the space between lines:</p>
<pre><code>p.small {  
line-height:  0.8;  
}  
  
p.big {  
line-height:  1.8;  
}
</code></pre>
<h2 id="text-direction">Text Direction</h2>
<p>The  <code>direction</code>  property is used to change the text direction of an element:</p>
<pre><code>p {  
direction:  rtl;  
}
</code></pre>
<h2 id="word-spacing">Word Spacing</h2>
<p>The  <code>word-spacing</code>  property is used to specify the space between the words in a text.</p>
<p>The following example demonstrates how to increase or decrease the space between words:</p>
<pre><code>h1 {  
word-spacing:  10px;  
}  
  
h2 {  
word-spacing:  -5px;  
}
</code></pre>
<h2 id="text-shadow">Text Shadow</h2>
<p>The  <code>text-shadow</code>  property adds shadow to text.</p>
<p>The following example specifies the position of the horizontal shadow (3px), the position of the vertical shadow (2px) and the color of the shadow (red):</p>
<pre><code>h1 {  
text-shadow:  3px 2px red;  
}
</code></pre>
<h1 id="css--fonts">CSS  Fonts</h1>
<p>The CSS font properties define the font family, boldness, size, and the style of a text.</p>
<h2 id="css-font-families">CSS Font Families</h2>
<ul>
<li>
<p><strong>generic family</strong>  - a group of font families with a similar look (like “Serif” or “Monospace”)</p>
</li>
<li>
<p><strong>font family</strong>  - a specific font family (like “Times New Roman” or “Arial”)</p>
</li>
<li>
<h2 id="font-family">Font Family</h2>
<pre><code>p {  
  font-family:  "Times New Roman", Times, serif;  
  }
</code></pre>
</li>
</ul>
<h2 id="font-style">Font Style</h2>
<p>The  <code>font-style</code>  property is mostly used to specify italic text.</p>
<p>This property has three values:</p>
<ul>
<li>normal - The text is shown normally</li>
<li>italic - The text is shown in italics</li>
<li>oblique - The text is “leaning” (oblique is very similar to italic, but less supported)</li>
</ul>
<h2 id="font-size">Font Size</h2>
<p>The <code>font-size</code> property sets the size of the text.</p>
<pre><code>h1 {  
font-size:  40px;  
}  
  
h2 {  
font-size:  30px;  
}  
  
p {  
font-size:  14px;  
}
</code></pre>
<h2 id="set-font-size-with-em">Set Font Size With Em</h2>
<p>To allow users to resize the text (in the browser menu), many developers use em instead of pixels.</p>
<pre><code>h1 {  
font-size:  2.5em;  /* 40px/16=2.5em */  
}  
  
h2 {  
font-size:  1.875em;  /* 30px/16=1.875em */  
}  
  
p {  
font-size:  0.875em;  /* 14px/16=0.875em */  
}
</code></pre>
<h1 id="css--icons">CSS  Icons</h1>
<h2 id="font-awesome-icons">Font Awesome Icons</h2>
<p>o use the Font Awesome icons, add the following line inside the  <code>&lt;head&gt;</code>  section of your HTML page:</p>
<p><code>&lt;link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"&gt;</code></p>
<h2 id="bootstrap-icons">Bootstrap Icons</h2>
<p>To use the Bootstrap glyphicons, add the following line inside the  <code>&lt;head&gt;</code>  section of your HTML page:</p>
<p><code>&lt;link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css"&gt;</code></p>
<h2 id="google-icons">Google Icons</h2>
<p>To use the Google icons, add the following line inside the  <code>&lt;head&gt;</code>  section of your HTML page:</p>
<p><code>&lt;link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons"&gt;</code></p>
<h1 id="css--links">CSS  Links</h1>
<h2 id="styling-links">Styling Links</h2>
<p>Links can be styled with any CSS property (e.g.  <code>color</code>,  <code>font-family</code>,  <code>background</code>, etc.).</p>
<pre><code>a {  
color:  hotpink;  
}
</code></pre>
<ul>
<li>
<p><code>a:link</code>  - a normal, unvisited link</p>
</li>
<li>
<p><code>a:visited</code>  - a link the user has visited</p>
</li>
<li>
<p><code>a:hover</code>  - a link when the user mouses over it</p>
</li>
<li>
<p><code>a:active</code>  - a link the moment it is clicked</p>
<p>/* unvisited link */<br>
a:link {<br>
color:  red;<br>
}</p>
<p>/* visited link */<br>
a:visited {<br>
color:  green;<br>
}</p>
<p>/* mouse over link */<br>
a:hover {<br>
color:  hotpink;<br>
}</p>
<p>/* selected link */<br>
a:active {<br>
color:  blue;<br>
}</p>
</li>
</ul>
<h2 id="text-decoration-1">Text Decoration</h2>
<p>The  <code>text-decoration</code>  property is mostly used to remove underlines from links:</p>
<pre><code>a:link {  
text-decoration:  none;  
}
</code></pre>
<h2 id="background-color-2">Background Color</h2>
<p>The <code>background-color</code> property can be used to specify a background color for links:</p>
<pre><code>a:link {  
background-color:  yellow;  
}
</code></pre>

