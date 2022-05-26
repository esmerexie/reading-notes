# CSS <img src="https://img.icons8.com/external-flaticons-lineal-color-flat-icons/344/external-css-computer-science-flaticons-lineal-color-flat-icons-2.png" width="40" height="40">
[CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/What_is_CSS) or Cascading Style Sheets helps allow you to design your website. When building a website I like to think of it as HTML being the skeleton and CSS being the asthetic to everything on top of the skeleton. But what do I mean by that you may ask? Well for starters you can change a color of a text by doing  

```
h1 {  
    color: red;
 }

```  

from the example given aboove, we started with a selecter in this case being `h1` following with the text color being `red`.  

Another example of design we could do is being able to change the font size. To do this we can write

```
h1 {
    color: red;
    font-size: 5em;
}

```

You can see by the example that not only did we change the color to red but now we chaged the `font-size` to `5em`.

## Two ways of adding CSS to HTML

1. The first and in my opinion the best way of adding CSS is by doing so `Externally`. You can start by adding a 
`style.css` file. By adding one of the example above to your new `style.css` file we can then add a link to our HTML connecting to our `style.css`. To do so adding this line 
```
<link rel="stylesheet" heref="style.css" />
```

1. Will now apply any design to the text you have added to the `style.css` file.

2. The second way to add CSS to your HTML file is to do so `Interanally`. For example to start, opening up your HTML file and adding your CSS code to the file instead having to writ the code in a serperate file or externally.  

```

h1 {  
    color: red;
 }
</style>
</head>
<body>

<h1>Hello</h1>

```  

This is just the scratch of the surface of what CSS is capable of but for more in-depth details you should vist [HERE](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/What_is_CSS) or if you are looking for a CSS cheat sheet [HERE](https://htmlcheatsheet.com/css/) would be a good starting point.