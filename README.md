1. Difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll

getElementById → Finds a single element with a specified id.

getElementsByClassName → Gets a list of all elements with a specified class name.

querySelector → Gets the first matching element using a CSS selector.

querySelectorAll → Gets a list of all matching elements using a CSS selector.

2. Rules for creating and adding new elements to the DOM

createElement is used to create a new element, then various methods such as appendChild or append are used to add that element to the DOM.

3. What is Event Bubbling and how does it work

Event Bubbling is a process where when an event occurs on a child element, it is propagated up to the parent element step by step.

4. What is Event Delegation and why is it needed

Event Delegation is a method of controlling events of its child elements by setting an event listener on the parent element. This is necessary so that a separate listener does not have to be set for each child element and even if a new child is added, it can be controlled from the parent.

5. Difference between preventDefault() and stopPropagation()

preventDefault() → Stops the browser's default behavior.

stopPropagation() → Prevents the event from propagating to the parent element.
