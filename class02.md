# Readings

## Chapter 2 Text

This chapter pg. 40-61 on **HTML & CSS by JON DUCKETT** basically went over new elements or tags we can use when writing in HTML. One of the exampls are *italics*

```html
<i> Your text here </i>
```

Another one would be Subscript and Superscript. An example of this would be writing CO<sub>2</sub> (sub) & E=MC<sup>2</sup> (sup). To write this use

```html
CO<sub>2</sub>

E=MC<sup>2</sup>

```

One of the tags that I found very useful and will try to implement in future projects are line breaks and horizontal lines. Specifically the horizontal line. The line below is an example of the horizontal line.

<hr />

When written it is used to seperate two different topics or sections.

```html
This tag is also known as an empty element
<hr />
and doesn't need a second tag to close.
```

To Cite a text or paragraph you can use

```html
<cite> </cite>
```

and you can define a word by using

```html
<dfn> </dfn>
```

When writing an address or an email you can use.

```html
<address>your address, contact info, and email goes here.</address>
```

## Chapter 10 Introducing CSS

This chapter introduces the basics of CSS and how to add life to our HTML code. When talking about adding life to our code I mean adding color, changing the font or style, adding borders to our text, and so much more!
There is two ways you can add CSS to your HTML code and that is **External** and **Internal**.

To summarize this wrting CSS externally is by making a seprate CSS file from your HTML and adding the style code through there.

To write CSS internally is to add CSS style to your HTML file.

Next was the topic on **CSS Selectors**. Selectors are basically ways to target HTML elements and write rules to them. There are many different types of selectors and some of them are

```css
type selector - matches element names
h1, h2, h3 {}

class selectors - matches an element whose class attribute has a value that matches the one specified after the period (or full stop) symbol.
.note {}
p.note {}
```

> One thing to note when writing rules on CSS is to understand how they cascade. If for example there are two rules written for one element the last rule will take precedent over the first rule.

<hr />

## Chapter 2 Basic Javascript Instructions

This chapter goes over basic Javascript instructions. Statements are a series of instructions that a computer can follow one-by-one. An example of a statement is one gotten from the book

```js
var today = new Date();
var hourNow= today.getHours();
var greeting;

if (hourNow > 18) {
    greeting = "Good evening";
}   else if (hourNow > 12) {
    greeting = "Good afternoon";
}   else if (hourNow > 0) {
    greeting = "Good morning";
}   else {
    greeting = "Welcome";
}
document.write(greeting);
```

You can also write comments using Javascript using

```js
/* this is a comment to explain how this comment works */
```

### Variables, when I think about variables I like to think about hot pockets. In order to have or delcare a variable you must give it a name and have contents inside of it. An example of this would be

```js
    var userName;               /* giving a variable a name */
    userName = "John";          /* storing data in the variable */
    userName()                  /* delcaring the variable */
```

### When thinking of data types there are 3 that Javascript distinguishes between. Those are **numbers**, **strings**, and true or false statements known as **Booleans**

An example of all three are

```js
1.50                    numeric data type
"Hello world!"          string data type
true                    boolean data type
```

There are rules for naming variables.

1. The name must begin with a letter, dollar sign ($), or an underscore (_).

2. The name can contains letters, numbers and special characters.

3. You cannot use special words i.e var

4. All variables are case sensitive

5. Use a name that describes the variable

6. If the variable is made up of more than one word, use a capital letter for the first letter of the word after the first word. thisIsAnExample

### Array is a special type of variable that allows you to store a list of vaules

### Expressions evaluates into a single vaule

for example

```js
    var color = "black";
    var area = 3 * 9;
```

Expressions rely on things called operators. They allow programmers to create a single value from one or more values. An example of this would be an arithmetic operator.

```js
    area = 3 * 2;
```

Javascript contains the following mathematical operators.

```js
addition +
subtraction -
division /
multiplication *
increment ++
decrement --
modulus %
```

## Chapter 4 Decisions and Loops

When writing a script there are often times where the code can take multiple paths. That is the decision making process and an easy visualization of that is a flowchart.

### Evaluating conditions & conditional statements

there are two components to a decision

1. An expression is evaluated, which returns a value
2. A conditional statement says what to do in a given situation

Evaluation of a condition is where your code checks the status of your scripts and depending on the two vaules given it will return a true or false vaule.

Conditional statements is based on a if/then/else statement. *if* the condition is met then the code executes, *else* your code does something different or just skips a step.

```js
    if (score > 50) {
        document.write("You passed!");
    }   else {
        document.write("Try again!");
    }
```

### Comparison operators: Evauluating conditions

You can evaluate a situation by comparing one or more vaule. The end result would be a true or false Boolean.

```js
== is equal to
!= is not equal to
=== strict equal to
!== strict not equal to
> greater than
< less than
>= greater than or equal to
<= less than or equal to
```

### if statements

This statement is simple. It evaluates a condition based on the code. If the condition evaluates to true then the line of code executes.

```js
if (score >= 50) {
    congratulations();
}
```

### *if else* statements

checks a condition. If the conditions is true then the code executes. If the condition is false then another set of code executes.

```js
if (score >= 50) {
    congratulations();
}
else {
    encourage();
}
```

### Switch Statements

Think of a classic puzzle game that has multple stages, in this case it would be three. In each stage, it gives you a message of encouragement. Starting from the first level being the highlest level of encouragement and gradually lowering as the user progress. This concept is simlar to the switch statement.

> A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that vaule.

For example

```js
var msg;            // Message
var level = 2;      // level

// Determin message based on level
switch (level) {
    case 1:
        msg = " Good luck on the first test";
        break;

        case 2:
        msg = " Good luck on the second test";
        break;

        case 3:
        msg = " Good luck on the third test";
        break;
}

var el = document.getElementById("answer");
el.textContent = msg;
```

## Things I want to know more about

I want to know more about switch statements and how to properly write them and on which oconditions will a developer use them.

I also want to know more about conditional statements and how to properly write them. I tried before in the past and in some instances my code would not run. Instead the code will break.
