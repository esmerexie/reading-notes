# Operators

operators are simple. They are the actions used to perform arithmetic on numbers. Exampls are  

```js
x + y (addition)
x - y (subtraction)
x * y (muliplication)
x / y (division)
x % y (modulus / division remainder)
```

For more symobls on operators visit this [site](https://www.w3schools.com/js/js_operators.asp).

## Loops

By definition [Loops](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration#while_statement) is a quick and easy way to do something repeatedly. Although efficient it is another way to show you how powerful a computer is. When typing the code

```js

while (true) {
  console.log('Hello, world!');
}

```

creates an infinite loop and doesn't break until said otherwise.  
But before going further on loops we should understand the different types. Although spelled differently they all essentially do the same thing.

> - a **for** statement repeats itself until the condition evaluates to false.
> - a **do while** statements repeats itself until the specified condition evaluates to false.

an example of a do while statement is

```js
let i = 0;
do {
  i += 1;
  console.log(i);
} while (i < 50000);
```

>NOTE : change the number 500000 beforehand unless wanting to see how powerful this loop is.

a while statement will continue to execute until the statement is true. You will see by the time that loop ends it will break the code causing it to stop cause the statement will eventually come true.
