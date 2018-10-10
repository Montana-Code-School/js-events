# JavaScript Events

### What is an Event?

An HTML event can be something the browser does, or something a user does.

Here are some examples of HTML events:

- An HTML web page has finished loading
- An HTML input field was changed
- An HTML button was clicked

Often, when events happen, you may want to do something.

[w3Schools.com - JavaScript Events](https://www.w3schools.com/js/js_events.asp)

### Registering Event Listeners

To execute JavaScript code when events are detected you need to register event listeners/handlers for the DOM element the event is occuring on.

There are multiple ways to register event listeners. Here are the two most common used approaches:

1. HTML Attribute

`<button onclick="alert('Hello World!')">`

2. addEventListener Method

```
// Assuming myButton is a button element
myButton.addEventListener('click', greet);

function greet(event){

  // print and have a look at the event object

  console.log('Hello World', event);
  alert('Hello World!')
}
```

[MDN - Events and the DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Events)

### DOM Event Types

There are many different HTML DOM events, some of the most commonly used are:

- blur
- change
- click
- load
- keyUp
- scroll

For a complete list of events review [w3Schools.com - DOM Events](https://www.w3schools.com/jsref/dom_obj_event.asp)

### More Resources

- [Medium - How to handle JS Events](https://medium.freecodecamp.org/event-handling-in-javascript-with-examples-f6bc1e2fff57)
- [Video - What Are Events in JS](https://www.youtube.com/watch?v=gx0oAgvXyE4)
- [MDN - DOM Event Interface ](https://developer.mozilla.org/en-US/docs/Web/API/Event)

### Exercises

Take a look at the index.html file in this repository. Open the file in the Chrome web browser. You should see a checkout page created with the Bootstrap CSS framework.

Let's create some user interactions by using JavaScript events. (Do not change the HTML itself to solve any exercises. Try to accomplish everything by using JavScript ;))

1. Alert 'Welcome to our Checkout! Glad you are buying your stuff from us.' when the HTML page has finished loading. Refresh the page.

2. Remove the event listener you created in the last exercise. Make sure no alert box pops up once you refresh the page.

3. Alert 'Promo Code Applied' if a user clicks the 'Redeem' button.

   1. Use the HTML attribute as your first solution
   2. Refactor your solution to use the addEventListener method

4. As soon as a user starts typing in the promo code text field, have the Promo code update on every key stroke. For example if a user starts typing "S" the text "EXAMPLECODE" should change to "S". If the user types the next letter "SU" the Promo code text should read "SU" and so forth.

5. If a user clicks or focuses on any text input field make the corresponding label to the input field should change to the color blue by applying the [class "text-primary"](https://getbootstrap.com/docs/4.1/utilities/colors/) to the label.

6. Let's build a simple form validation:
   1. If a user clicks on the "Continue to checkout" button check if any text input fields are empty.
   2. If a text input field is empty apply the [class "is-invalid"](https://getbootstrap.com/docs/4.1/components/forms/#validation) to it.
