### This is the README file for the HTML project.

### Table of Contents
* [Getting Started](https://github.com/valikmed/FreeCodeCamp/blob/main/HTML/Day%201/README.md)
* [File Structure](#file-structure)
* [Examples](#examples)

### Getting Started
To get started, open the index.html file in a web browser.

### File Structure
The project consists of the following files and folders:

* index.html: The main HTML file.
* README.md: This file.

#Day 1

### Examples
H - hyper
T - text
M - markup
L - language

HTML:        Content/Structure
CSS:         Styling
JavaSript:   Interactivity

Attributes
*An attribute is a value placed inside the opening tag of the HTML element.
Attributes provide additional information about the element or specify how the element should behave.*


###### Example 1:
`<div id="root"></div>`
Where `<div>` is a tag that is open and ready to pass `id` that is an attribute and `"root"`  that is a value and at the end we need to close our tag by writing `</div>`.

###### Example 2:
`<a href="https://www.example-website.com">Visit our website</a>`

All in tag `<a></a>` is an element, and `href` is an attribute inside of we have value that is `"https://www.example-website.com"` link


###### Example 3:
`<img src="image.jpg" alt=" A beautiful image" />` why we haven't tag that close tag when we open, it is because `<img />` tag is void type

All in tag `<img />` is an element.
`src` and `alt` are attributs
`"image.jpg"` and `"A beautiful image` are values


###### Example 4:

`<input type="checkbox" checked />` all in `<input />` is element with type `void`. 
`type` and `checked` are attributes, and `checked` is boolean attribute like `disabled`
`"checkbox"` is value

# Day 2
###### Example 5:
```html
<h1 id="title">Movie Review Page</h1>
```

`id` is attribute of `h1` element and always must be unique
we can referens to `id` in JavaScript or CSS by
```css
#title {
color: red;
}
```

```html
<div class="box"></div> 

<div class="box red"></div> <!-- you can add multiple class names ans separate them with a space -->

```

The way to access classes names attribute
```css
.box {
width: 200px;
heigth: 200px;
border: 2px solid black;
}
```

- Classes are best used when you want to apply a set of styles to many elements
- If you want to target a specific element, it is best to use an id

##### HTML entity
*An HTML entity, or character reference, is a set of characters used to represent reserved characters in HTML*

Correct HTML entities for the less-than and greater-than symbols
```html
<p>This is an &lt;img /&gt; element</p>
```

`&#60`; - decimal numeric reference
`&#c3C`; - hexadecimal numeric reference

*What are some other examples of using HTML entities?*
- Copyright symbol
- Quotes
- Trademark symbol
- Ampersand sign

*What is the link element?*
The link element links to external resources like stylesheets and site icons.

```html
<!-- Using the link element for an external CSS file -->
<link rel="stylsheet" href="./styles.css" />
```

```html
<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
		<title>Examples of the link element </title>
		<link rel="stylesheet" href="./styles.css" />
		<link rel="preconnect" href="https:/fonts.googleapis.com" />
		<link rel="preconnect" href="https:/fonts.gstatic.com" crossorigin />
	</head>
	<body>
	</body>
</html>
```
Or another typical use case of link
```html
<link rel="icon" href="favicon.ico" />
```

##### The Script Element
*Used to embed executable code. Most developers will use this to execute JavaScript code.*
- interactive
- image sliders
- dynamic forms

Using the script element in an HTML document
```html
<body>
	<script>
		alert("Welcome to my web site")
	</script>
</body>
```

Or we can do this

```JavaScript
alert("Welcome to my web site")
```

After that, we reuse its code in our HTML like this

```html
<body>
	<script src='PATH:\User\Folder\File\JavaScript\fileWithAlert'></script>
</body>
```


##### UTF-8
*UTF-8, or UCS Transformation Format 8, is a standardized character encoding widely used on the web.*

All  text on the web page is a sequence of characters stored as 1 or more bytes.

A byte is a unit of data consisting of 8 bits, or binary digits


##### SEO - Search Engine Optimization
SEO is a practice that optimizes web pages so they become more visible and rank higher in search engines.

```html
<meta name="description" content="Discover expert tips and techniques for gardening in small spaces, choosing the right plans, and maintaining a thriving garden." />
```


##### Open Graph protocol
The open graph protocol enables you to control how your website's content appears across various social media platforms such as Facebook and LinkedIn.

```html
<meta content="myWebSite.com" property="og:title" />
<!-- or -->
<meta property="og:type" content="website" />
<!-- or -->
<meta content="https://cdn.freecodecamp.org/platform/universal/fcc_meta_1920X1080-indigo.png" property="org:image"/>
<!-- or -->
<meta property="or:url" content="https://www.freecodecamp.org" />
```

There are more OG properties that you can set
`og:description`, `og:audio`, `og:video`, `og:locale`
