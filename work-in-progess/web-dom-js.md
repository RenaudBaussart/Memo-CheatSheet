## Parent Child and Sibling
children – only those children that are element nodes.

firstElementChild, lastElementChild – first and last element children.

previousElementSibling, nextElementSibling – neighbor elements.

parentElement – parent element.
## Tables
The `<table>` element supports (in addition to the given above) these properties:

    table.rows – the collection of <tr> elements of the table.
    table.caption/tHead/tFoot – references to elements <caption>, <thead>, <tfoot>.
    table.tBodies – the collection of <tbody> elements (can be many according to the standard, but there will always be at least one – even if it is not in the source HTML, the browser will put it in the DOM).

`<thead>, <tfoot>, <tbody>` elements provide the rows property:

    tbody.rows – the collection of <tr> inside.

`<tr>`:

    tr.cells – the collection of <td> and <th> cells inside the given <tr>.
    tr.sectionRowIndex – the position (index) of the given <tr> inside the enclosing <thead>/<tbody>/<tfoot>.
    tr.rowIndex – the number of the <tr> in the table as a whole (including all table rows).

`<td>` and `<th>`:

    td.cellIndex – the number of the cell inside the enclosing <tr>.
## query
document.getElementById - get the position of a selected id(dont do global id?. id = one specifique element)

elem.querySelectorAll - selecte all element inside the selected scope

elem.querySelector - return the first element selected in the scope

elem.matches - return true of false if the scope matche the selected element

elem.closest - this methode look the the nearest ancestor that match the scope
## Dom properties

instanceof - return a true if is inherited 

innerHTML - property allows to get the HTML inside the element as a string.We can also modify it. So it’s one of the most powerful ways to change the page.

outerHTML - property contains the full HTML of the element. That’s like innerHTML plus the element itself.

textContent - provides access to the text inside the element: only text, minus all <tags>

elem.hasAttribute(name) – checks for existence.

elem.getAttribute(name) – gets the value.

elem.setAttribute(name, value) – sets the value.

elem.removeAttribute(name) – removes the attribute
### get element by
There are also other methods to look for nodes by a tag, class, etc.

Today, they are mostly history, as querySelector is more powerful and shorter to write.

So here we cover them mainly for completeness, while you can still find them in the old scripts.

    elem.getElementsByTagName(tag) looks for elements with the given tag and returns the collection of them. The tag parameter can also be a star "*" for “any tags”.

    elem.getElementsByClassName(className) returns elements that have the given CSS class.

    document.getElementsByName(name) returns elements with the given name attribute, document-wide. Very rarely used.
## modifying the document

document.createElement(tag) - Creates a new element node with the given tag

document.createTextNode(text) - Creates a new text node with the given text
### insertion methode
element.append() - insert the scope in the element
    Here are more insertion methods, they specify different places where to insert:

    node.append(...nodes or strings) – append nodes or strings at the end of node,
    node.prepend(...nodes or strings) – insert nodes or strings at the beginning of node,
    node.before(...nodes or strings) –- insert nodes or strings before node,
    node.after(...nodes or strings) –- insert nodes or strings after node,
    node.replaceWith(...nodes or strings) –- replaces node with the given nodes or strings.

elem.insertAdjacentHTML(where, html).
The first parameter is a code word, specifying where to insert relative to elem. Must be one of the following:

    "beforebegin" – insert html immediately before elem,
    "afterbegin" – insert html into elem, at the beginning,
    "beforeend" – insert html into elem, at the end,
    "afterend" – insert html immediately after elem.

The second parameter is an HTML string, that is inserted “as HTML”.
### removal methode
node.remove() - remove a node

### clone node
elem.cloneNode(true) creates a “deep” clone of the element – with all attributes and subelements. If we call elem.cloneNode(false), then the clone is made without child elements

DocumentFragment -  is a special DOM node that serves as a wrapper to pass around lists of nodes.We can append other nodes to it, but when we insert it somewhere, then its content is inserted instead

### write
document.write() - write what is in the scope right here and nowz
## dom node classes
The classes are:

    EventTarget – is the root “abstract” class for everything.

    Objects of that class are never created. It serves as a base, so that all DOM nodes support so-called “events”, we’ll study them later.

    Node – is also an “abstract” class, serving as a base for DOM nodes.

    It provides the core tree functionality: parentNode, nextSibling, childNodes and so on (they are getters). Objects of Node class are never created. But there are other classes that inherit from it (and so inherit the Node functionality).

    Document, for historical reasons often inherited by HTMLDocument (though the latest spec doesn’t dictate it) – is a document as a whole.

    The document global object belongs exactly to this class. It serves as an entry point to the DOM.

    CharacterData – an “abstract” class, inherited by:
        Text – the class corresponding to a text inside elements, e.g. Hello in <p>Hello</p>.
        Comment – the class for comments. They are not shown, but each comment becomes a member of DOM.

    Element – is the base class for DOM elements.

    It provides element-level navigation like nextElementSibling, children and searching methods like getElementsByTagName, querySelector.

    A browser supports not only HTML, but also XML and SVG. So the Element class serves as a base for more specific classes: SVGElement, XMLElement (we don’t need them here) and HTMLElement.

    Finally, HTMLElement is the basic class for all HTML elements. We’ll work with it most of the time.

    It is inherited by concrete HTML elements:
        HTMLInputElement – the class for <input> elements,
        HTMLBodyElement – the class for <body> elements,
        HTMLAnchorElement – the class for <a> elements,
        …and so on.

## element size and scroll
    offsetParent – is the nearest positioned ancestor or td, th, table, body.

    offsetLeft/offsetTop – coordinates relative to the upper-left edge of offsetParent.

    offsetWidth/offsetHeight – “outer” width/height of an element including borders.

    clientLeft/clientTop – the distances from the upper-left outer corner to the upper-left inner (content + padding) corner. For left-to-right OS they are always the 
    widths of left/top borders. For right-to-left OS the vertical scrollbar is on the left so clientLeft includes its width too.

    clientWidth/clientHeight – the width/height of the content including paddings, but without the scrollbar.

    scrollWidth/scrollHeight – the width/height of the content, just like clientWidth/clientHeight, but also include scrolled-out, invisible part of the element.
    
    scrollLeft/scrollTop – width/height of the scrolled out upper part of the element, starting from its upper-left corner.
   
