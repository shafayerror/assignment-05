# README

## 6. JavaScript DOM & Events -- Q&A

### 1. What is the difference between `getElementById`, `getElementsByClassName`, and `querySelector / querySelectorAll`?

-   **`getElementById`** returns a single element that matches the given
    ID. IDs are unique in a document, so this always gives at most one
    element.\
-   **`getElementsByClassName`** returns a live HTMLCollection of all
    elements that have the specified class.\
-   **`querySelector`** returns the first element that matches a CSS
    selector.\
-   **`querySelectorAll`** returns a static NodeList of all elements
    that match a CSS selector.

------------------------------------------------------------------------

### 2. How do you create and insert a new element into the DOM?

To insert a new element, you first create it using
`document.createElement()`. Then you can set its attributes, text, or
styles. Finally, you attach it to the document by using methods like
`appendChild`, `prepend`, or `insertBefore`.

------------------------------------------------------------------------

### 3. What is Event Bubbling and how does it work?

Event Bubbling is the process where an event triggered on a child
element propagates upward to its parent, then the parent's parent, and
continues up to the root of the document unless it is stopped.

------------------------------------------------------------------------

### 4. What is Event Delegation in JavaScript? Why is it useful?

Event Delegation is a technique where instead of attaching event
listeners to multiple child elements, you attach a single listener to a
common parent. The parent listens for events that bubble up from its
children and handles them conditionally. This is useful because it
reduces memory usage, simplifies code, and also works for dynamically
added child elements.

------------------------------------------------------------------------

### 5. What is the difference between `preventDefault()` and `stopPropagation()` methods?

-   **`preventDefault()`** stops the browser's default action for a
    particular event, such as preventing a link from navigating or a
    form from submitting.\
-   **`stopPropagation()`** prevents the event from moving further along
    the bubbling or capturing phases, stopping it from reaching other
    event listeners on parent elements.
