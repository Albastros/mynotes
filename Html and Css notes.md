# Html, Css, Scss

# **What is HTML?**

HTML stands for **H**yper **T**ext **M**arkup **L**anguage

HTML is the **standard markup** language for Web pages

HTML **elements** are the building blocks of HTML pages

HTML elements are represented by **<> tags**

# HTML Elements

An HTML element is a **start** tag and an **end** tag with content in between:

<h1>This is a Heading</h1>

| Start tag | Element content | End tag |
| --- | --- | --- |
| <h1> | This is a Heading | </h1> |
| <p> | This is paragraph. | </p> |

# HTML Attributes

- HTML elements can have **attributes**
- Attributes provide **additional information** about the element
- Attributes come in name/value pairs like **charset="utf-8"**

# A Simple HTML Document

```jsx
<!DOCTYPE html>
<html lang="en">

<meta charset="utf-8">
<title>Page Title</title>

<body>
   <h1>This is a Heading</h1>
   <p>This is a paragraph.</p>
   <p>This is another paragraph.</p>
</body>

</html>
```

# Example Explained

HTML elements are the building blocks of HTML pages.

- The `<!DOCTYPE html>` declaration defines this document to be HTML5
- The `<html>` element is the root element of an HTML page
- The `lang` attribute defines the language of the document
- The `<meta>` element contains meta information about the document
- The `charset` attribute defines the character set used in the document
- The `<title>` element specifies a title for the document
- The `<body>` element contains the visible page content
- The `<h1>` element defines a large heading
- The `<p>` element defines a paragraph

---

# HTML Documents

All HTML documents must start with a document type declaration: `<!DOCTYPE html>`.

The HTML document itself begins with `<html>` and ends with `</html>`.

The visible part of the HTML document is between `<body>` and `</body>`.

# HTML Headings

HTML headings are defined with `<h1>` to `<h6>` tags.

`<h1>` defines the most important heading. `<h6>` defines the least important heading:

```jsx
<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<h3>This is heading 3</h3>
```

# Example

```jsx
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
```

# HTML Paragraphs

HTML paragraphs are defined with `<p>` tags:

# Example

```jsx
<p>This is a paragraph.</p><p>This is another paragraph.</p>
```

# HTML Links

HTML links are defined with `<a>` tags:

# Example

```jsx
<a href="https://www.nathnaelmesfin.com">This is a link</a>
```

The link's destination is specified in the `href` attribute.

# HTML Images

HTML images are defined with `<img>` tags.

The source file (`src`), alternative text (`alt`), `width`, and `height` are provided as attributes:

# Example

```jsx
<img src="nathnaelmesfin.jpg" alt="nathnaelmesfin" style="width:120px;height:150px"
```

# HTML Buttons

HTML buttons are defined with `<button>` tags:

# Example

```jsx
<button>Click me</button>
```

# HTML Lists

HTML lists are defined with `<ul>` (unordered/bullet list) or `<ol>` (ordered/numbered list) tags, followed by `<li>` tags (list items):

# Example

```jsx
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

# HTML Tables

An HTML table is defined with a `<table>` tag.

Table rows are defined with `<tr>` tags.

Table headers are defined with `<th>` tags. (bold and centered by default).

Table cells (data) are defined with `<td>` tags.

# Example

```jsx
<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>50</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>94</td>
  </tr>
</table>
```

# Programming HTML

Every HTML element can have **attributes**.

For web development and programming, the most important attributes are **id** and **class.** These attributes are often used to address program based web page manipulations.

| Attribute | Example |
| --- | --- |
| id | <table id="table01" |
| class | <p class="normal"> |
| style | <p style="font-size:16px"> |
| data- | <div data-id="500"> |
| onclick | <input onclick="myFunction()"> |
| onmouseover | <a onmouseover="this.setAttribute('style','color:red')"> |

# **What Is CSS?**

CSS stands for Cascading Style Sheets language and is used to stylize elements written in a markup language such as HTML. It separates the content from the visual representation of the site. The relation between HTML and CSS is strongly tied together since HTML is the very foundation of a site and CSS is all of the aesthetics of an entire website.

# **CSS Advantages on Web Pages**

The difference between a web page that implements CSS and one that doesn’t is massive and surely noticeable.

You might have seen a website that fails to load completely and has a white background color with most of the text being blue and black. This means that the CSS part of the web page didn’t load correctly or it doesn’t exist altogether.

That’s what web pages with only HTML look like, and I think you’d agree that that’s not very appealing.

Before using CSS, all of the stylizing had to be included into the HTML markup. This means web developers had to separately describe the background color, font size, alignments, etc.

CSS lets you stylize everything on a different file, thus creating the design there and later on integrating the CSS files on top of the HTML markup. This makes the actual HTML markup much cleaner and easier to maintain.

In short, with CSS features you don’t need to repeatedly describe how individual elements look. This saves time, shortens the code, and makes it not as prone to errors.

CSS lets you have multiple styles on one HTML page, therefore making the customization possibilities almost endless. Nowadays, this is becoming more a necessity than a commodity.

# **How Does CSS Work?**

CSS uses a simple English based syntax with a set of rules that govern it. Like we’ve mentioned before, HTML was never intended to use style elements, only the markup of the page. It was created to merely describe the content. For example: **<p>This is a paragraph.</p>**.

But how do you style the paragraph? The CSS syntax structure is pretty simple. It has a selector and a declaration block. You select an element and then declare what you want to do with it. Pretty straightforward, right?

However, there are rules you have to remember. The structure rules are pretty simple, so don’t worry.

The selector points to the HTML elements you want to style. The declaration block contains one or more declarations separated by semicolons.

Each declaration includes a CSS property name and a value, separated by a colon. A CSS declaration always ends with a semicolon, and declaration blocks are surrounded by curly braces.

Let’s look at an example:

All of the **<p>** elements will be colored blue and bolded.

```jsx
<style>

p {

color: blue;

text-weight: bold;

}

<style>
```

In another example, all **<p>** elements will be center-aligned, be 16x wide and pink.

```jsx
<style>

p {

text-align: center;

font-size: 16px;

color: pink;

}

</style>
```

See our **[CSS cheat sheet](https://www.hostinger.com/tutorials/css-cheat-sheet)** for more examples.

Now let’s talk about the different styles of CSS. They are Inline, External and Internal.

# **Internal, External and Inline CSS Styles**

We’ll go over each style briefly, for an in-depth explanation of each method, there will be a link below the overview.

Let’s start by talking about the **Internal** style. CSS styles done this way are loaded each time an entire website is refreshed, which may increase loading time. Additionally, you won’t be able to use the same CSS style on multiple pages as it’s contained within a single page. However, this also comes with benefits. Having everything on one page makes it easier to share the template for a preview.

The **External** method might be the most convenient one. Everything is done externally on a **.css** file. This means you can do all the styling on a separate file and apply the CSS to any page you want. The External style might also improve loading times.

Lastly, we will talk about the **Inline** style of CSS. Inline works with specific elements that have the <style> tag. Each component has to be stylized, so it might not be the best or fastest way to handle CSS. But it can come in handy. For example, if you want to change a single element, quickly preview changes, or maybe you don’t have access to the CSS files.

# **Scss**

**SCSS** stands for **Sassy CSS**, which is a preprocessor scripting language that is interpreted or compiled into Cascading Style Sheets (CSS). It is a more powerful version of CSS that allows us to use variables, nested rules, mixins, functions, and more, all with a fully CSS-compatible syntax.

The main advantage of using SCSS is that it makes the process of writing CSS easier and more efficient. With its nested syntax, you can write less code and improve the readability and organization of your stylesheet. Additionally, you can use mixins and variables to quickly and easily reuse styles across your codebase, which can save time and reduce errors.

other advantages of using SCSS is that it allows you to write more modular and maintainable CSS code through the use of reusable code blocks and variables. Additionally, the nesting feature in SCSS allows for more structured and readable code by visually indicating the hierarchy of your styles.

SCSS files are typically compiled into CSS files before being deployed to a website or web application, using a compiler such as Sass or a task runner like Grunt or Gulp.

SCSS also includes features like `@import` and `@extend` to help you manage your stylesheet more effectively. These features allow you to break your CSS into smaller, more manageable files, and to easily reuse styles between different elements.

Overall, SCSS is a powerful tool that can help you write more efficient, organized, and maintainable CSS code.

**What is the difference between CSS and SCSS ?**

- **Syntax:** CSS follows a plain-text syntax, whereas SCSS follows a more structured syntax with additional features such as variables, nesting, and mixins.
- **Variables:** SCSS allows you to define variables to store commonly used values such as colors, font sizes, and spacing, whereas CSS does not.
- **Nesting:** SCSS allows you to nest selectors within other selectors, making it easier to write and read complex stylesheets, whereas CSS requires you to write each selector separately.
- **Mixins:** SCSS allows you to create reusable code snippets using mixins, which are like functions in programming languages. CSS does not provide this functionality.
- **File Extension:** CSS files use the .css file extension, while SCSS files use the .scss file extension.
- **Compilation:** CSS files are interpreted by web browsers directly, whereas SCSS files must be preprocessed into standard CSS files using a preprocessor such as Sass.
- SCSS contains all the features of CSS and contains more features that are not present in CSS which makes it a good choice for developers to use it.
- SCSS offers variables, you can shorten your code by using variables. It is a great advantage over conventional CSS.
