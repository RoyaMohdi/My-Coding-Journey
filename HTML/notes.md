# HTML Learning Notes

> 👩‍💻 My personal notes as I learn HTML, with examples, quizzes, and challenges!

##  🗺️ My Learning Progress
- [x] 1. Introduction
- [X] 2. Basic Structure
- [x] 3. Nested Elements
- [x] 4. Attributes
- [x] 5. Headings
- [x] 6. Paragraphs
- [x] 7. Styles
- [x] 8. Text Formatting
- [x] 9. Quotations & Citations
- [ ] 10. Comments
- [ ] 11. Colors & CSS
- [ ] 12. Links & Images
- [ ] 13. Tables & Lists
- [ ] 14. Forms

---
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

| Tag | What it does |
|---|---|
| `<!DOCTYPE html>` | Defines the document as HTML5 |
| `<html>` | The root element of the page |
| `<head>` | Contains information about the page (not visible) |
| `<title>` | The title shown in the browser tab |
| `<body>` | Contains everything visible on the page |
| `<h1>` | A main heading |
| `<p>` | A paragraph |


> 🏠 **Memory trick:** `<html>` is the whole house, `<head>` is the attic (hidden stuff),
> and `<body>` is the rooms everyone can see.

### What is an Element?
An element is everything from the start tag to the end tag:
```html
<tagname>Content goes here...</tagname>
```
- **Empty elements** have no content and no end tag, like `<br>` (line break).
- HTML is **not case-sensitive**, but lowercase is recommended.

### 🧠 Quick Quiz
**Q: Which part of the page is visible to users: `<head>` or `<body>`?**
<details>
<summary>👀 Click to see the answer</summary>

`<body>` 🎉 The `<head>` holds hidden information like the title.
</details>

---

## 🪆 3. Nested HTML Elements

HTML elements can be **nested**, meaning an element can contain other elements.

```html
<body>
    <h1>Welcome</h1>
    <p>This is my webpage.</p>
</body>
```

The `<h1>` and `<p>` elements are nested inside `<body>`.

> 🪆 **Think of nesting like Russian dolls:** each element fits inside another one.

> [!WARNING]
> Never skip the end tag! `<p>Hello` ❌ → `<p>Hello</p>` ✅
> Close tags in the **opposite order** you opened them: `<p><b>Hi</b></p>` ✅

---

## 🏷️ 4. HTML Attributes

- Attributes give **extra information** about elements.
- They go in the **opening tag**.
- They use name/value pairs: `name="value"`.

| Attribute | Used with | What it does | Example |
|---|---|---|---|
| `href` | `<a>` | Link destination | `<a href="https://www.google.com">Google</a>` |
| `src` | `<img>` | Image location | `<img src="cat.jpg">` |
| `alt` | `<img>` | Text if image can't load | `<img src="cat.jpg" alt="A cute cat">` |
| `width` / `height` | `<img>` | Image size in pixels | `<img src="cat.jpg" width="300">` |
| `style` | Any element | Inline CSS styling | `<p style="color: red;">Hi</p>` |
| `lang` | `<html>` | Language of the page | `<html lang="en">` |
| `title` | Any element | Tooltip on hover | `<p title="Hello!">Hover me</p>` |

> [!TIP]
> Always write attributes in **lowercase** and put values in **"quotes"**.
> Always add `alt` to images; it helps people using screen readers.

### 🧠 Quick Quiz
**Q: Which attribute tells a link where to go?**
<details>
<summary>👀 Click to see the answer</summary>

`href` 🎉 (Memory trick: **h**yperlink **ref**erence)
</details>

---


## 🔠 5. HTML Headings

```html
<h1>Heading 1</h1>  <!-- Biggest and most important -->
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>  <!-- Smallest -->
```
- `<h1>` = most important, `<h6>` = least important.
- Search engines use headings to understand your page.

> 📰 **Think of a newspaper:** `<h1>` is the big front-page headline, `<h2>` are section titles, and `<h3>` are article titles.

> [!TIP]
> Use only **one** `<h1>` per page, and don't use headings just to make text big.

---
## 📄 6. HTML Paragraphs

| Tag | What it does |
|---|---|
| `<p>` | A paragraph (adds space before and after) |
| `<br>` | A line break, without a new paragraph |
| `<hr>` | A horizontal line to separate content |
| `<pre>` | Preformatted text that keeps spaces and line breaks |

```html
<p>This is a paragraph.</p>
<hr>
<p>This is a line<br>break inside a paragraph.</p>
<pre>
Text in pre
   keeps    spaces!
</pre>
```
> [!NOTE]
> Browsers **ignore** extra spaces and new lines in your code. Use `<br>` or `<pre>` to control them.

---

## 🎨 7. HTML Styles

The `style` attribute adds color, fonts, and size:
```html
<tagname style="property: value;">
```

| Property | What it changes | Example |
|---|---|---|
| `background-color` | Background color | `style="background-color: powderblue;"` |
| `color` | Text color | `style="color: blue;"` |
| `font-family` | Font | `style="font-family: Arial;"` |
| `font-size` | Text size | `style="font-size: 20px;"` |
| `text-align` | Alignment | `style="text-align: center;"` |

### 🎯 Challenge
Make a heading that is **purple**, **centered**, and uses the **Verdana** font.
<details>
<summary>👀 Click to see the solution</summary>

```html
<h1 style="color: purple; text-align: center; font-family: Verdana;">My Heading</h1>
```
</details>

---





