# Dynamic web pages with Javascript

## What is [Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)?

> Javascript is a lightweight, interpreted, or compiled programming language with first-class functions.

Or to be more specific

- prototype-based
- multi paradigm
- single-threaded
- dynamic language
- supporting object-oriented
- imperative
- and declarative styles.

## Input Output in plain JavaScript

when thinking of input and output what comes to your mind? Well I like to think of it as giving something and then getting a result for giving that thing `(whatever that thing may be)`. An example that can be given is a simple textbox that a user recieves, then inputs their answer to the question or a simple text box with pre-requisits of filling out then recives the output or the result for the answer to the question or the fill-ins to the text box. A bit confusing? Yes, I know. Too many words were used, to put it into a simple perspective or an example : 

- user logs into website
- website askes for user's name
- user enter credentials 
- website produces message to user

or another example is to show you a code from my very own `app.js` file which can be tested and viewed at [Here](esmerexie.github.io/fruits/).

```
let askMessage = prompt("Do you like fruits?");
if (askMessage == "yes")
    document.write("Hello, fellow fruit person!");
    else if (askMessage == "no")
    document.write("Hello, non-fruit person!");
    else if (askMessage =="")
    document.write("So you do not have a name?")
```

Let me try my best to explain whats going on here. On the very first line the website when loading into the very first time will produce a text message and you will be prompted with a message "Do you like fruits?".  
`let askMessage = prompt("Do you like fruits?")`  
If your answer was `yes` then the output will be "Hello, fellow fruit person!"

```

if (askMessage == "yes")  
    document.write("Hello, Fellow fruit person!")
```

Now if your answer was `no` then the result would be "Hello, non-fruit person!"

```

else if (askMessage == "no")
    document.write("Hello, non-fruit person!");
```

Last but not least if you had no answer and left the text field blank and hit `enter`, you would get the message "So you do not have a name?"

```
else if (askMessage =="")
    document.write("So you do not have a name?")
```