# Readings

## HTML Forms

>Why are forms so important in web development?

I think the reason why forms are so important in webt development because it provides feedback and data to the Dev from the user.

> When designing a form, what are some key things to keep in mind when it comes to user experience?

To keep the userinterface design simple and straight to the point. Having the design too complicated might frustrate users.

> List 5 form elements and explain their importance.

1. Form Element - is like a container storing all of the form elemnts.

2. label - is a used for every text field in our form.

3. input - is used for the user to have the ability to input certain information.

4. text area - is a multiline text area.

5. button - is an element that holds 3 vaules. Submit where data is sent defined by the action attribute of the form element. Reset which resets all of the form widgets to their default value immediately. And button which does nothing.

## Learn JS

> How would you describe events to a non-technical friend?

- Events are like signals to do something. You code something to do a specific task which lets your computer execute the task.

> When using the addEventListener() method, what 2 arguments will you need to provide?

- The name of the event and a function to handle the event

> Describe the event object. Why is the target within the event object useful?

- event,evt, or e objects when used autmatically passed to event handlers to provide extra features and information.

> What is the difference between event bubbling and event capturing?

- Event bubbling is the exact opposite of the event capturing. When an event is fired on an element that has parent elements, modern browsers run three different phases. Capturing, target, and bubbling phase.

```html
The target phase:

The browser checks to see if the element's outer-most ancestor (<html>) has a click event handler registered on it for the capturing phase, and runs it if so.

Then it moves on to the next element inside <html> and does the same thing, then the next one, and so on until it reaches the direct parent of the element that was actually clicked.

The bubbling phase:

The browser checks to see if the direct parent of the clicked element has a click event handler registered on it for the bubbling phase, and runs it if so.
Then it moves on to the next immediate ancestor element and does the same thing, then the next one, and so on until it reaches the <html> element.
```

Information is refferenced [Here](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)

## Things I want to know more about

I want to know more about events and go a little more in depth.
