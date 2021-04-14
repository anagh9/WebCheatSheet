# WebCheatSheet
# HTML TUTORIAL

---

### Headings

```Heading
<h1> Hello World! </h1>
<h2> Hello World! </h2>
<h3> Hello World! </h3>
<h4> Hello World! </h4>
<h5> Hello World! </h5>
<h6> Hello World! </h6>

```

### Structure

```Structure
<h1>Main title</h1>
<p>Introduction</p>
    <h2>Reasons</h2>
        <h3>Reason 1</h3>
        <p>Paragraph</p>

        <h3>Reason 2</h3>
        <p>Paragraph</p>

    <h2>In conclusion</h2>
    <p>Paragraph</p>


```

### Paragraphs

```Paragraphs
<p> Define a paragraph
<br> Insert a Single line break
<pre> Define pre-formatted text

```

### Highlighting

```
<mark> This text will be highlighted </mark>
<strong> This text will be Bold </strong>
<b> This text will be Bold </b>
<i> This text will be itylic </i>
<em> This text will be itylic </em>
<u> This text will be underlined </u>
```

### Abbreviation

```
<p>I like to write <abbr title="Hypertext Markup Language">HTML</abbr>!</p>
```

### Anchors and Hyperlinks

```
href : Specifies the destination address

----
<a href="http://example.com/">Link to example.com</a>
<a href="tel:11234567890">Call us</a>
<a href="javascript:myFunction();">Run Code</a>
<a href="#" onclick="myFunction(); return false;">Run Code</a>
<a href="mailto:example@example.com">Send email</a>
<a href="mailto:example@example.com?subject=Example+subject&body=Message+text">Send email</a>
---

rel : Specifies the relationship between the current document and the linked document

---
<a href="http://example.com/" rel="external">example site</a>
---

target : Specifies where to open the link, e.g. in a new tab or window. Possible values are _blank, _self,
_parent, _top, and framename (deprecated). Forcing such behaviour is not recommended since it
violates the control of the user over a website.

---
<a href="example.com" target="_blank">Text Here</a>
---
title : Specifies extra information about a link
download : Specifies that the target will be downloaded when a user clicks on the hyperlink. The value of the attribute will be the name of the downloaded file.

```

## Lists

---

### Ordered List

```
<ol>
    <li>Item</li>
    <li>Another Item</li>
    <li>Yet Another Item</li>
</ol>

Manually Changing the Number

<ol start="3">
    <li>Item</li>
    <li>Some Other Item</li>
    <li>Yet Another Item</li>
</ol>

Reversing

<ol reversed>
    <li>Item</li>
    <li>Some Other Item</li>
    <li value="4">A Reset Item</li>
    <li>Another Item</li>
    <li>Yet Another Item</li>
</ol>

Changing the type of numeral

<ol type="1|a|A|i|I">

1 Default value - Decimal numbers 1,2,3,4
a Alphabetically ordered (lowercase) a,b,c,d
A Alphabetically ordered (uppercase) A,B,C,D
i Roman Numerals (lowercase) i,ii,iii,iv
I Roman Numerals (uppercase) I,II,III,IV

```

### Unordered List

```
<ul>
    <li>Item</li>
    <li>Another Item</li>
    <li>Yet Another Item</li>
</ul>

Nested List

<ul>
    <li>item 1</li>
    <li>item 2
    <ul>
        <li>sub-item 2.1</li>
        <li>sub-item 2.2</li>
    </ul>
    </li>
    <li>item 3</li>
</ul>
```

### Description List

```
<dl>
    <dt>name 1</dt>
    <dd>value for 1</dd>
    <dt>name 2</dt>
    <dd>value for 2</dd>
</dl>

Output
---
name 1
    value for 1
name 2
    value for 2

```

## Tables

---

## Simple Table

```
<table>
    <tr>
        <th>Heading 1/Column 1</th>
        <th>Heading 2/Column 2</th>
    </tr>
    <tr>
        <td>Row 1 Data Column 1</td>
        <td>Row 1 Data Column 2</td>
    </tr>
    <tr>
        <td>Row 2 Data Column 1</td>
        <td>Row 2 Data Column 2</td>
    </tr>
</table>

Output
---
-------------------------------------------------
Heading 1/Column 1    | Heading 2/Column 2      |
----------------------|--------------------------
Row 1 Data Column 1   |   Row 1 Data Column 2   |
Row 2 Data Column 1   |   Row 2 Data Column 2   |
-------------------------------------------------

```

## Spanning columns or rows

```
<table>
    <tr>
        <td>row 1 col 1</td>
        <td>row 1 col 2</td>
        <td>row 1 col 3</td>
    </tr>
    <tr>
        <td colspan="3">This second row spans all three columns</td>
    </tr>
    <tr>
        <td rowspan="2">This cell spans two rows</td>
        <td>row 3 col 2</td>
        <td>row 3 col 3</td>
    </tr>
    <tr>
        <td>row 4 col 2</td>
        <td>row 4 col 3</td>
    </tr>
</table>
```

![Output](https://raw.githubusercontent.com/anagh9/WebCheatSheet/master/1.JPG)

## Table with thead, tbody, tfoot, and caption

---

```
<table>
    <caption>Table Title</caption> <!--| caption is the first child of table |-->
    <thead> <!--======================| thead is after caption |-->
        <tr>
            <th>Header content 1</th>
            <th>Header content 2</th>
        </tr>
    </thead>

    <tbody> <!--======================| tbody is after thead |-->
        <tr>
            <td>Body content 1</td>
            <td>Body content 2</td>
        </tr>
    </tbody>

    <tfoot><!--| tfoot can be placed before or after tbody, but not in a group of tbody. |-->
<!--| Regardless where tfoot is in markup, it is rendered at the bottom. |-->
        <tr>
            <td>Footer content 1</td>
            <td>Footer content 2</td>
        </tr>
    </tfoot>
</table>
```

![Output](https://raw.githubusercontent.com/anagh9/WebCheatSheet/master/2.JPG)

## Comments

```
<!-- I'm an HTML comment! -->
```

## Images

| Parameters  |                                            Details                                            |
| ----------- | :-------------------------------------------------------------------------------------------: |
| src         |                                Specifies the URL of the image                                 |
| srcset      |  Images to use in different situations (e.g., high-resolution displays, small monitors, etc)  |
| sizes       |                                Image sizes between breakpoints                                |
| crossorigin |                         How the element handles crossorigin requests                          |
| usemap      |                                   Name of image map to use                                    |
| alt         | Alternative text that should be displayed if for some reason the image could not be displayed |
| width       |                          Specifies the width of the image (optional)                          |
| height      |                         Specifies the height of the image (optional)                          |

```
<img src="images/hello.png" alt="Hello World">
<img src="https://i.stack.imgur.com/ALgZi.jpg?s=48&g=1" alt="StackOverflow user Caleb Kleveter">

<img sizes="(min-width: 1200px) 580px,
(min-width: 640px) 48vw,
98vw"
srcset="img/hello-300.jpg 300w,
img/hello-600.jpg 600w,
img/hello-900.jpg 900w,
img/hello-1200.jpg 1200w"
src="img/hello-900.jpg" alt="hello">
```

## Responsive image using picture element

```
<picture>
    <source media="(min-width: 600px)" srcset="large_image.jpg">
    <source media="(min-width: 450px)" srcset="small_image.jpg">
    <img src="default_image.jpg" style="width:auto;">
</picture>
```

## Input Control Elements

---

| Parameters   |                                                                                                                                                           Details                                                                                                                                                           |
| ------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| class        |                                                                                                                                              Indicates the Class of the input                                                                                                                                               |
| id           |                                                                                                                                                Indicates the ID of the input                                                                                                                                                |
| type         | Identifies the type of input control to display. Acceptable values are hidden, text, tel, url, email,password, date, time, number, range, color, checkbox, radio, file, submit, image, reset, and button.Defaults to text if not specified, if the value is invalid, or if the browser does not support the type specified. |
| name         |                                                                                                                                               Indicates the name of the input                                                                                                                                               |
| disabled     |                                                                                  Boolean value that indicates the input should be disabled. Disabled controls cannot be edited, are not sent on form submission, and cannot receive focus.                                                                                  |
| checked      |                                                                        When the value of the type attribute is radio or checkbox, the presence of this Boolean attribute indicates that the control is selected by default; otherwise it is ignored                                                                         |
| placeholder  |                                                                                            HTML5 A hint to the user of what can be entered in the control . The placeholder text must not contain carriage returns or line-feeds                                                                                            |
| autocomplete |                                                                                                               HTML5 Indicates whether the value of the control can be automatically completed by the browser                                                                                                                |
| required     |                                                                                                        HTML5 Indicates a value must be present or the element must be checked in order for the form to be submitted                                                                                                         |
| alt          |                                                                                                                               An alternative text for images, in case they are not displayed.                                                                                                                               |
| step         |                                                                                The step attribute specifies the legal number intervals. It works with the following input types: number, range, date, datetime-local, month, time and week.                                                                                 |

```
<input type="text">
<input type="text" size="50">

Checkbox and Radio Buttons
---
<input type="checkbox">
<input type="radio">
<input type="radio" name="color" id="red" value="#F00">
<input type="radio" name="color" id="green" value="#0F0">
<input type="radio" name="color" id="blue" value="#00F">
<input checked>
<input checked="">
<input checked="checked">
<input checked="ChEcKeD">
<input type="radio">
<input type="checkbox">

```

## Labels

---

- To give context to the buttons and show users what each button is for, each of them should have a label. This can be done using a <label> element to wrap the button. Also, this makes the label clickable, so you select the corresponding button

---

```
<label>
    <input type="radio" name="color" value="#F00">
    Red
</label>

<input type="checkbox" name="color" value="#F00" id="red">
<label for="red">Red</label>
```

## Button Groups

- Since each radio button affects the others in the group, it is common to provide a label or context for the entire group of radio buttons.
- To provide a label for the entire group, the radio buttons should be included in a {fieldset} element with a {legend} element within it.

```
<fieldset>
    <legend>Theme color:</legend>
    <p>
        <input type="radio" name="color" id="red" value="#F00">
        <label for="red">Red</label>
    </p>
    <p>
        <input type="radio" name="color" id="green" value="#0F0">
        <label for="green">Green</label>
    </p>
    <p>
        <input type="radio" name="color" id="blue" value="#00F">
        <label for="blue">Blue</label>
    </p>
</fieldset>

```

## Input Validation

```
Use the required attribute to indicate that a field must be completed in order to pass validation.

<input required>
<input minlength="3">
<input maxlength="15">
<input minlength="3" maxlength="15">
<input pattern="\d*" title="Numbers only, please.">
<input type="color" name="favcolor" value="#ff0000">
```

## Form Basics

```
<form>
    <input type="text" name="name" required>
    <input type="email" name="email" required>
    <input type="password" name="password">
    <input pattern="\d*" name="number" required>

    <input type="submit" value="Publish"> <!-- form will be validated -->
    <input type="submit" value="Save" formnovalidate> <!-- form will NOT be validated -->
</form>

<form action="upload_file.php" method="post" enctype="multipart/form-data">
Select file to upload:
    <input type="file" name="fileSubmission" id="fileSubmission">
    <input type="submit" value="Upload your file" name="submit">
</form>
```

## Button

```
<input type="button" value="Button Text">
<input type="button" onclick="alert('hello world!')" value="Click Me">
<button type="button" onclick="alert('hello world!')">Click Me</button>
<input type="submit" value="Submit">

<button type="submit">
    <img src="submit-icon.jpg" /> Submit
</button>

<input type="tel" value="+8400000000">

<form>
    <label>E-mail: <label>
    <input type="email" name="email">
</form>

<input type="search" name="googlesearch">

<input type="image" src="img.png" alt="image_name" height="50px" width="50px"/>


```

## Forms

#### Submitting

```
<form action="action.php">
```

- The method attribute is used to define the HTTP method of the form which is either GET or POST.

```
<form action="action.php" method="get">
<form action="action.php" method="post">
```

#### Uploading Files

- Images and files can be uploaded/submitted to server by setting enctype attribute of form tag to multipart/formdata.
  enctype specifies how form data would be encoded while submitting to the server.

```
<form method="post" enctype="multipart/form-data" action="upload.php">
    <input type="file" name="pic" />
    <input type="submit" value="Upload" />
</form>

```

## Grouping a few input fields

```
<form>
    <fieldset>
        <legend>1st field set:</legend>
            Field one:<br>
        <input type="text"><br>
            Field two:<br>
        <input type="text"><br>
    </fieldset><br>
    <fieldset>
        <legend>2nd field set:</legend>
            Field three:<br>
        <input type="text"><br>
            Field four:<br>
        <input type="text"><br>
    </fieldset><br>
    <input type="submit" value="Submit">
</form>
```

![Output](https://raw.githubusercontent.com/anagh9/WebCheatSheet/master/3.JPG)

## Media Elements

### Audio

```
<audio controls>
    <source src="file.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
</audio>
```

### Video

```
<video width="500" height="700" controls>
    <source src="video.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
```

## Video header or background

```
<video width="1280" height="720" autoplay muted loop poster="video.jpg" id="videobg">
    <source src="video.mp4" type="video/mp4">
    <source src="video.webm" type="video/webm">
    <source src="video.ogg" type="video/ogg">
</video>

#videobg {
    background: url(video.jpg) no-repeat;
    background-size: cover;
}

```

### Selection Menu Controls

```
The <select> element generates a drop-down menu from which the user can choose an option.

<select name="">
    <option value="1">One</option>
    <option value="2">Two</option>
    <option value="3">Three</option>
    <option value="4">Four</option>
</select>

<select name="" size="4"></select>
```

### Datalist

```
<input list="Languages">
Language HTML
<datalist id="Languages">
    <option value="PHP">
    <option value="Perl">
    <option value="Python">
    <option value="Ruby">
    <option value="C+">
</datalist>

```

### Embed

```
<embed src="myflash.swf">
<embed type="video/mp4" src="video.mp4" width="640" height="480">
```

### IFrames

```
<iframe sandbox src="http://example.com/"></iframe>
<iframe src="base.html"></iframe>
<iframe src="base.html" width="800" height="600"></iframe>
```

### Meta Information

#### Page Information

Giving the name of the Web application that the page represents.

```
<meta name="application-name" content="OpenStreetMap">

author:
<meta name="author" content="Your Name">

description:
<meta name="description" content="Page Description">

keywords:
<meta name="keywords" content="Keyword1, Keyword2">

socialMedia:
<meta property="fb:app_id" content="123456789">
<meta property="og:url" content="https://example.com/page.html">
<meta property="og:type" content="website">
<meta property="og:title" content="Content Title">
<meta property="og:image" content="https://example.com/image.jpg">
<meta property="og:description" content="Description Here">
<meta property="og:site_name" content="Site Name">
<meta property="og:locale" content="en_US">
<meta property="article:author" content="">

Mobile Layout Control:
<meta name="viewport" content="width=device-width, initial-scale=1">

Automatic Refresh:
<meta http-equiv="refresh" content="5">

Phone Number Recognition:
<meta name="format-detection" content="telephone=no">
```

## Marking up computer code

```
<pre>
    <code>
    x = 42
    if x == 42:
        print "x is … … 42"
    </code>
</pre>

<pre>
    <code>
        &lt;p>This is a paragraph.&lt;/p>
    </code>
</pre>

<p>The <code>a</code> element creates a hyperlink.</p>
```
