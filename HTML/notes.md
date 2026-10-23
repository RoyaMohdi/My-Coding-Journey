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

**Image attribute:**
```html
<img src="image.jpg" alt="My image">
```
- `src` specifies the image location.
- `alt` provides alternative text for the image.

**Style attribute:**
```html
<p style="color: red;">Hello World</p>
```
- `style` adds inline CSS styling.

**Language attribute:**
```html
<html lang="en">
``
HTML Quotation and Citation Elements
<blockquote> that is quoted from another source 
<q> defines a short quotation
<abbr> defins an abbreviation or an acronym like "HTML:. "CSS", "Mr",…
<address> defines the contact information for the author/owner of the document or an article.
<cite> defines the title of a creative work, 
<bdo>bi- Directional Override : use to overrid the current text directions


