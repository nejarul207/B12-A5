Question-1 : What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

Answer : getElementById : selects one element by ID, returns a single element.

         getElementsByClassName : selects all elements with a class, returns a live HTMLCollection.
         
         querySelector : selects the first element matching any CSS selector, returns a single element.
         
         querySelectorAll : selects all elements matching any CSS selector, returns a static NodeList.

Question-2 : How do you create and insert a new element into the DOM?

Answer : const newDiv = document.createElement("div");
         newDiv.textContent = "Hello!";
         document.body.appendChild(newDiv);

Question-3 : What is Event Bubbling and how does it work?

Answer : Event Bubbling is a process where an event that happens on a child element “bubbles up” and triggers the same event on its parent elements in the DOM hierarchy.

         How it works: 1. An event occurs on a target element.
                       2. The event first triggers on that element.
                       3. Then it propagates upward to its parent, then grandparent, and so on, up to the document root.
                       4. All ancestors with listeners for that event will be notified unless propagation is stopped with event.stopPropagation().

Question-4 : What is Event Delegation in JavaScript? Why is it useful?

Answer : Event Delegation is when you listen for events on a parent element instead of each child. The event automatically bubbles up from the child to the parent, letting you handle it there.
         Why it’s useful: 1. Efficiency: Reduces the number of event listeners.
                          2. Dynamic elements: Works for elements added to the DOM after the listener is attached.
                          3. Simpler code: Easier to manage events for many child elements.

Question-5 : What is the difference between preventDefault() and stopPropagation() methods?

Answer : Difference between preventDefault() and stopPropagation() methods:
         1. preventDefault(): Stops the browser’s default action for an event but does not stop event propagation.
         2. stopPropagation(): Stops the event from bubbling or capturing through the DOM but does not prevent the default browser action.
         
    
         
