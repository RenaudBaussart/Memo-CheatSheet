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
        </header>
        <footer>
        </footer>
    </body>
</html>
```
## HTML5 specific tag
- `<header>`: Defines the header block for a document or a section
- `<footer>`: Defines the footer block for a document or a section
- `<main>`: Describes the main content of a document
- `<article>`: Identifies an article inside a document
- `<aside></aside>`: Specifies content contained in a document sidebar
- `<section></section>`: Defines a section of a document
- `<details></details>`: Describes additonal information that user can view or hide
- `<dialog></dialog>: A dialog box or a window
- `<figure></figure>: An independent content block featuring images, diagrams or illustrations
- `<figcaption></figcaption>: Caption that describe a figure
- `<mark></mark>`: Displays a portion of highlighted text with in a page content
- `<nav></nav>`: Navigation links for the user in a document
- `<menuitem></menuitem>`: The specific menu item that a user can raise from a pop up menu
- `<meter></meter>`: Describes the scalar measurement with in a known array
- `<progress></progress>`: Displays the progress of a task usually a progress bar
- `<rp></rp>`: Describes text within the browsers that do not support ruby notations
- `<rt></rt>`: Displays east asian typography character details
- `<ruby></ruby>`: Describes annotations for east asian typography
- `<summary></summary>`: Contains a visible heading for details element
- `<bdi></bdi>`: Helps you format parts of text in a different direction than other text
- `<time></time>`: Identifies the time and date
- `<wbr>`: A line break within the content
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
- `<input>`: make a zone were you can put stuff inside
    - example:  
        ```
        <label for="name">Name (4 to 8 characters):</label>
        <input type="text" id="name" name="name" required minlength="4" maxlength="8" size="10" />
        ```
    - `<input type="radio">`: collections of radio buttons describing a set of related options (look like of a dropdown in the foctionality)
        - example:
            ```
            <fieldset>
            <legend>Select a maintenance drone:</legend>

            <div>
                <input type="radio" id="huey" name="drone" value="huey" checked />
                <label for="huey">Huey</label>
            </div>

            <div>
                <input type="radio" id="dewey" name="drone" value="dewey" />
                <label for="dewey">Dewey</label>
            </div>

            <div>
                <input type="radio" id="louie" name="drone" value="louie" />
                <label for="louie">Louie</label>
            </div>
            </fieldset>
            ```
    - `<input type="checkbox">`: same as radio but in a checkbox style
        - example:
            ```
            <fieldset>
              <legend>Choose your monster's features:</legend>

                <div>
                    <input type="checkbox" id="scales" name="scales" checked />
                    <label for="scales">Scales</label>
                </div>

                <div>
                    <input type="checkbox" id="horns" name="horns" />
                  <label for="horns">Horns</label>
                </div>
            </fieldset>
            ```
- `<textarea>`: Textarea
- `<label>`: to make a checkbox
    - example:
    ```
    <label for="cheese">Do you like cheese?</label>
    <input type="checkbox" name="cheese" id="cheese" />
    ```
- `<select>`: use to make a dropdown menu for a answer option
    - exemple:
    ```
        <label for="pet-select">Choose a pet:</label>
        <select name="pets" id="pet-select">
          <option value="">--Please choose an option--</option>
          <option value="dog">Dog</option>
          <option value="cat">Cat</option>
          <option value="hamster">Hamster</option>
          <option value="parrot">Parrot</option>
          <option value="spider">Spider</option>
          <option value="goldfish">Goldfish</option>
        </select>

    ```
- `<button>`: create a buton element
    - exemple: `<button type="button">Add to favorites</button>`
- `<video>` : add a video box
    - example:
    ```
    <video controls width="250">
        <source src="/media/cc0-videos/flower.webm" type="video/webm" />

        <source src="/media/cc0-videos/flower.mp4" type="video/mp4" />

        Download the
        <a href="/media/cc0-videos/flower.webm">WEBM</a>
        or
        <a href="/media/cc0-videos/flower.mp4">MP4</a>
        video.
    </video>
    ```
## Common HTML Attributes

- `id`: Unique identifier
- `class`: Class name for styling
- `href`: Hyperlink reference
- `src`: Source (e.g., for images)
- `alt`: Alternate text for images
- `title`: Tooltip text