# Readings

All information written on this document was taken from *HTML & CSS, JAVASCRIPT & JQUERY by Jon Duckett*.

## Chapter 3 Lists

In this chapter I learned that there are 3 main different types of lists when it comes to HTML.

```html
<ol> </ol> // ordered list
<ul> </ul> // unordered list
<dl> </dl> // definition list
```

## Chapter 13 Boxes

In this chapter we read about how CSS affects our HTML code. Starting out with box dimensions and limiting width and height.

```css
h {
    height: 1px;
    width: 1px;
}

i {
    min-width: 1px;
    max-width: 2px;
}

i {
    min-height: 1px;
    max-height: 1px;
}
```

Of course these are all examples so trying it out yourself is the best way to figure out how things work!

I then read about border, margin and padding! In summary each box that you create has 3 properties that can be edjusted to control its appearance. **BORDER, MARGIN, and PADDING**.

Another important thing talked about in this chapter was **White space and Vertical margin**. With this added to your HTML code you can add space between items on the page instead of having borders close together.

```css

l {
    width: 1px;
    height: 2px;
}

l_two {
    padding: 10px;
}
```

I learned that trying to center something to a screen can take many developers to try and figure out because there are many ways to try and do it!

### Box Shadows

One of the other things that I can recall from this chapter was the ability to add box shadows. It does what it means. It adds a shadow to the existing box that you have made to add some style to it!

### Box styles

On top of creating boxes and or shadows, you don't have to stick with plain old straight corners! You can make the corners rounded or have elliptical shapes.

## Review Chapter 2 Basic Javascript Instructions

In this chapter that I have already read, we just went over and reviewed again specific contents in this chapter.

## Arrays

Arrays allows the developer to create a list of vaules. Specifically, when creating a list that is related to eachother, the developer should consider using this. Below is an example of an array

```js

var colors;
colors = ['red', 'blue', 'yellow'];

ver el = document.getElementById('colors');
el.textContent = colors[0];

```

You can also store vaules in arrays. For example, red = [0], blue = [1], and yellow = [2]. When coding it is important to know that when counting up, you should always start with 0.

## Chapter 4 Decisions and loops

*if else* statements checks a condition. If the condition is true then the first line of code is executed. If the condition is to be false, then the second line of code is to be executed.

```js

if (score >=25) {
    congratulate();
}
else {
    encourage();
}
```

### Switch Statements

A switch statement basically starts with a variable. Then it is given a set of values and whichever vaule matches with the variable, the code is then to be exectued. An example of this is

```js

switch(level1) {
    case 'Zero':
        title = "Level 0";
        break;
    
    case "One":
        title = "Level 1";
        break;
    
    case "Two":
        title = "Level 2";
        break;
    
    default:
        title = "Test";
        break;
}
```

### Truthy and falsy vaules

> Every value in Javascript can  be treated as if it were true or false.

```js

Falsy Value

var lowscore = false;
var lowscore = 0;
var lowscore = "";
var lowscore = 1/"score";
var lowscore = 

Truthy Value

var lowscore = true;
var lowscore = 1;
var lowscore = "correct";
var lowscore = 3/6;
var lowscore = "true";

```

## Loops

Loops basically checks a condition. If the condition returns true, then it continues to run till the condition returns false.

```js

for (var i = 0; i < 10; i++) {
    document.write(i);
}

```

## Things I want to know more about

I want to know more about properly using loops and when to use switches. I also want to learn how to write cleaner code and their proper uses.
