## HTML
## Basic Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Title of the Document</title>
</head>
<body>

<header>
    <h1>Heading</h1>
    <nav>
        <ul>
            <li><a href="#section1">Section 1</a></li>
            <li><a href="#section2">Section 2</a></li>
            <li><a href="#section3">Section 3</a></li>
        </ul>
    </nav>
</header>

<section id="section1">
    <h2>Section 1</h2>
    <p>Content here.</p>
</section>

<section id="section2">
    <h2>Section 2</h2>
    <p>Content here.</p>
</section>

<section id="section3">
    <h2>Section 3</h2>
    <p>Content here.</p>
</section>

<footer>
    <p>&copy; Year | Footer content</p>
</footer>

</body>
</html>
```
## Common HTML Tags

- `<h1>` - `<h6>`: Headings
- `<p>`: Paragraph
- `<a>`: Anchor (Link)
- `<img>`: Image
- `<div>`: Division
- `<span>`: Inline Division
- `<ul>`: Unordered List
- `<ol>`: Ordered List
- `<li>`: List Item
- `<table>`: Table
- `<tr>`: Table Row
- `<td>`: Table Data
- `<form>`: Form
- `<input>`: Input
- `<textarea>`: Textarea

## Common HTML Attributes

- `id`: Unique identifier
- `class`: Class name for styling
- `href`: Hyperlink reference
- `src`: Source (e.g., for images)
- `alt`: Alternate text for images
- `title`: Tooltip text

## Form Elements

```html
<form>
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>
    <br>
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>
    <br>
    <input type="submit" value="Submit">
</form>
