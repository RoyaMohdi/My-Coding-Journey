# HTML Learning Notes

## 1. Introduction to HTML

- HTML stands for **HyperText Markup Language**.
- HTML is the standard markup language used to create web pages.
- HTML consists of a series of elements.
- HTML elements tell the browser how to display content.

## 2. Basic HTML Structure

```html
<!DOCTYPE html>
<html>
<head>
    <title>My First Webpage</title>
</head>
<body>
    <h1>My First Heading</h1>
    <p>My First Paragraph</p>
</body>
</html>
```

### Explanation
- `<!DOCTYPE html>` — Defines the document as HTML5.
- `<html>` — The root element of the HTML page.
- `<head>` — Contains information about the webpage.
- `<title>` — Defines the title displayed in the browser tab.
- `<body>` — Contains the visible content of the webpage.
- `<h1>` — Defines a main heading.
- `<p>` — Defines a paragraph.

### HTML Element
An element is everything from the start tag to the end tag:
```html
<tagname>Content goes here...</tagname>
```
- Some elements have **no content and no end tag**. These are called **empty elements**, for example `<br>` (line break).
- HTML is **not case-sensitive**, but lowercase is recommended.

## 3. Nested HTML Elements

HTML elements can be nested, meaning an element can contain other elements.

**Example:**

```html
<body>
    <h1>Welcome</h1>
    <p>This is my webpage.</p>
</body>
```

The `<h1>` and `<p>` elements are nested inside the `<body>` element.

> ⚠️ Never skip the end tag. Some browsers still display the page correctly, but it can cause unexpected errors.

## 4. HTML Attributes

- HTML elements can have attributes.
- Attributes provide additional information about elements.
- Attributes are usually specified in the opening tag.
- Attributes commonly use name/value pairs: `name="value"`.

### Examples

**Link attribute:**
```html
<a href="https://www.google.com">Visit Google</a>
```
- `href` specifies the link destination.

**Image attributes:**
```html
<img src="image.jpg" alt="My image" width="500" height="300">
```
- `src` specifies the image location.
- `alt` provides alternative text if the image can't be displayed (also used by screen readers).
- `width` and `height` specify the image size in pixels.

**Style attribute:**
```html
<p style="color: red;">Hello World</p>
```
- `style` adds inline CSS styling.

**Language attribute:**
```html
<html lang="en">
```
- `lang` declares the language of the webpage. It helps search engines and screen readers.

**Title attribute:**
```html
<p title="I'm a tooltip">Hover over me</p>
```
- `title` shows extra information as a tooltip when you hover over the element.

### Attribute Tips
- Always use **lowercase** attribute names.
- Always put attribute values in **quotes**.

## 5. HTML Headings

- Headings are defined with `<h1>` to `<h6>`.
- `<h1>` is the most important heading and `<h6>` is the least important.

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

- Search engines use headings to understand the structure of a page.
- Use headings for structure only, not to make text big or bold.

## 6. HTML Paragraphs

- The `<p>` element defines a paragraph.
- Browsers automatically add space before and after a paragraph.
- Extra spaces and line breaks in the code are **ignored** by the browser.

```html
<p>This is a paragraph.</p>
<hr>
<p>This is a line<br>break inside a paragraph.</p>
<pre>
Text in a pre element
   keeps    spaces
and line breaks.
</pre>
```

- `<hr>` — Defines a horizontal line (thematic break).
- `<br>` — Defines a line break without starting a new paragraph.
- `<pre>` — Defines preformatted text that keeps spaces and line breaks.

## 7. HTML Styles

The `style` attribute is used to add styles such as color, font, and size.

```html
<tagname style="property:value;">
```

### Examples
```html
<body style="background-color: powderblue;">
<h1 style="color: blue;">This is a heading</h1>
<p style="font-family: Arial;">This is a paragraph.</p>
<p style="font-size: 20px;">Bigger text</p>
<p style="text-align: center;">Centered text</p>
```

- `background-color` — Background color
- `color` — Text color
- `font-family` — Font
- `font-size` — Text size
- `text-align` — Text alignment

## 8. HTML Text Formatting

| Tag | Meaning |
|---|---|
| `<b>` | Bold text |
| `<strong>` | Important text (bold) |
| `<i>` | Italic text |
| `<em>` | Emphasized text (italic) |
| `<mark>` | Highlighted text |
| `<small>` | Smaller text |
| `<del>` | Deleted (crossed-out) text |
| `<ins>` | Inserted (underlined) text |
| `<sub>` | Subscript text, like H<sub>2</sub>O |
| `<sup>` | Superscript text, like x<sup>2</sup> |

- `<strong>` and `<em>` add **meaning** (importance), which helps screen readers, while `<b>` and `<i>` only change the look.

## 9. HTML Quotation and Citation Elements

| Tag | Meaning |
|---|---|
| `<blockquote>` | A section quoted from another source |
| `<q>` | A short inline quotation (browsers add quotation marks) |
| `<abbr>` | An abbreviation or acronym, like "HTML", "CSS", "Mr." |
| `<address>` | Contact information for the author/owner of a document or article |
| `<cite>` | The title of a creative work (book, song, movie, painting) |
| `<bdo>` | Bi-Directional Override: overrides the current text direction |

### Examples
```html
<blockquote cite="https://www.example.com">
  This text is quoted from another website.
</blockquote>

<p>She said: <q>Practice makes perfect.</q></p>

<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>

<address>
  Written by Roya Mohammadi<br>
  Toronto, Canada
</address>

<p><cite>The Scream</cite> by Edvard Munch.</p>

<bdo dir="rtl">This text will be written from right to left</bdo>
```

- `title` in `<abbr>` shows the full meaning when you hover.
- `<address>` and `<cite>` usually display in *italic*.
- `dir="rtl"` means right-to-left; `dir="ltr"` means left-to-right.
