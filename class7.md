# Programming with JavaScript

When programming with JavaScript it is important to know about [Control flow](https://developer.mozilla.org/en-US/docs/Glossary/Control_flow). Now what is **Control flow**?  

> Control flow is the order in which the computer executes statements in a script.

In basic conditions, code will run from top to bottom unless given in more advance code which requires the code to change the control flow. In such cases it uses **conditional** statements or **if** or **else** statements. For an example of a if and else statement :

```js

if (askMessage == "yes/no") {
    document.write("text that responds to user asnwer here.");
} else {
    askMessage = "other than the wanted response text goes here";
    document.write(askMessage);
}
```

To understand what is going on here one thing to note is that I forgot to add the code when a user is prompted to enter something. To get a better understanding what I mean go [Here](https://esmerexie.github.io/fruits/). When first loading into the website you are being prompted with a message. Once you have submitted your response, you are then given feedback based on your answer. The same thing is happening here in this code. The user is prompted with a question, the user responds to question, then the user is given a response depending on the answer.

## Functions  

To best understand Functions go [HERE](https://www.w3schools.com/js/js_functions.asp).

Functions can be used on a variety of things and can be very powerful. Here is an example of one

```js
function mathFunction(a, b) {
    let total = a + b;
    console.log(total);
}
mathFunction(1, 2);
```

This is just a bare bone example of a function. We have the command **function** and the name given for the function witch is **mathFunction**. We have now given the **mathFunction** variables **a** and **b**. The last line returns and gives us the result of **a + b**.

`return` statment means the function will stop executing once the line reaches `return`. For more on functions go [HERE](https://www.w3schools.com/js/js_functions.asp).
