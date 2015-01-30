# JS TRAINING 

******

## What you will need

1. Browser ( Chrome, Safari, Firefox, IE, etc… )
2. Text Editor ( Sublime, Atom, TextEdit, Notepad, etc… )
3. Terminal
4. Git
5. jQuery Library


******

## Quick Overview HTML

******

###What is HTML?

HTML or HyperText Markup Language is the standard markup language 
used to create web pages. It is written in the form of HTML elements consisting 
of tags enclosed in angle brackets

******

### How does it work?


HTML consists different type of elements which are called tags. Some of those tags are:

******

```html
<div></div>
```

which defines the contaner. It stands for division. 
 
```html
<p></p>
```

Which is a paragraph container and stands for parapraph

```html
<a href="#"></a>
``` 
Which is a link and stands for anchor tag

And many more…

******

Each time you insert a new tag it acts like a box.
It will take a new line and will be under one another unless you specify it with javascript or css to do something else. 

But not all of the html tags are for division and space control. Some of them are about making the text italic or bold. Those tags do not take space just modify the content within the tag or modify the document itself. 

******

### What does an HTML document consist of?

******

```html
<!DOCTYPE html>
<html>
  <head></head>
  <body></body>
</html>
```

******

```html
<!DOCTYPE html>
```


This tag defines that this document is an html document and it also specifies implicitly the version number of this html document. In this case it is HTML 5

******

```html
<html>
</html>
```

This tag contains html related tags within it. It has two main elements. __<head>__ and __<body>__

******

```html
<head></head>
```

Head tag contains the information about the web page like the __Title__ and the required files for this page, like the __CSS__, and the __JavaScript__ files.

******

```html
<body></body>
```
The Body tag is where the content resides. Basically it contains all of the content you would like to show to the user. 

******


## Quick Overview CSS


******

CSS stands for Cascading Style Sheet. This documents only purpose is to style your html document. 

******
### How does it works?

******

The rules on the css files is applied by the browsers. The browser reads the html document and finds all the required documents like css and applies the rules based on the tag name, class name, or id name, of the element. 

******

## JavaScript


******

### What is JavaScript

******

JavaScript is a computer programming language commonly used to create interactive effects within web browsers. 

Recently JavaScript is also used for server side applications like Rails, PHP, Java, C#, etc…

******
### History

* JavaScript is developed by Brendan Eich for Netscape Commnucator in 1995. Netscape wanted to have a lightweight language to work on the client side to run Java Applets to adopt users from Microsofts Internet Explorer, whihc was Netscapes direct competition.  
* There is no connection between Java and JavaScript except the syntax adoption. 
* Not so successful in the beginning. It got very popular when javascript introduced ajax requests in 2005.

******
### Basics

******

#### Syntax


******
```javascript
var x = 5;
var y = 6;
var z = x + y;
```

******

__Comments__
Comments are code that are not executed. They are escaped and not evaluated by the computer.
They are usually used for explaning what the code block does. You can write comments in javascript as such:

```javascript
var x = 44; // I am assigning 44 to variable x
// var x = 2; I have to get rid of this line

/*
I am a comment and I like it :) 
*/

```

******

### Data Types

******
__Strings__

Strings are data types which is a collection of sequential characters in quotes (double or single). A string may include letters, digits, and various special characters.

```javascript
var string = 'I am a string';

var js = "(dʒɑːvəˌskrɪpt"; // Thats how you pronounce javascript apparently
```

******

__Numbers__


Numbers are numeric characters. JavaScript has only one type of numbers.

```javascript
var x = 5; 
var y = 5.05;
```

******

__Arrays__


Arrays are data structures that contains multiple elements within.

```javascript
var x = [5, 4, "Hello", "google"]; 
```
If you want to access to an array element you must call it with its index:

```javascript
x[0];
=> 5
x[3];
=> "google"
x[6];
=> undefined
```

******


__Booleans__


Boolean data types are a binary variables that can have one of two possible values, 0 (false) or 1 (true).
Booleans are often used in conditional testing.

```javascript
var x = true;
var y = false;
```
******




### Variables
JavaScript variables are containers for data values

```javascript
var x = 5;
var y = 6;
var z = x + y;
```

******

### Operators

******

__Assignment__
To assign a value to a variable we use a single "=" character. Everthing to the right of the "=" will be assigned to the right of the "="

```javascript
var z = x + y;
var q = x + 5;
y = y + 5;
```

******


__Arithmetic Operators__
Arithmetic operators are used to perform arithmetic between variables and/or values.

```javascript
var z = ( x + y ) * ( 10 / 2 ) + ( 10 - 2) ;
```

"+" for addition 
"-" for substraction
"/" for division
"*" for multiplication


******

__Conditionals Operators__


Conditional operators are operators that evaluate the value on the right of the operator to the value on the left of the operator

```javascript
5 === 5; // Checks for equality of the values
5 !== 4; // Checks if the values are not equal to each other
5 > 4; // Checks if 5 bigger than 4
5 < 4; // Checks if 5 smaller than 4
5 <= 4; // Checks if 5 smaller or equal to 4
5 >= 4; // Checks if 5 bigger or equal to 4
```
Conditional operators will always return __true__ or __false__ as a return value

******

### Conditionals

******

__if else__

if else method is used to check a value is something that we want or not and if so to run a code. 



```javascript
var number_one = 5;
var number_two = 5;
var answer;

if ( number_one === number_two) {
    answer = "Yes " + number_one + " is equal to " + number_two;
} else {
    answer = "No, for some reason " + number_one + " is not equal to " + number_two;
}
```


******

### Loops

Loops are used to run the same code again and again until the loops condtion is met. 
There are several loops but we will focus on only 2 of them

******


__For Loops__

```javascript
for (i = 0; i < 5; i++) {
    text = "The number is " + i;
}
```

******
__While Loops__

```javascript
while (i < 10) {
    text = "The number is " + i;
    i++;
}
```

******


### Functions 
Functions are code blocks that are called as a method to execute the code within and return a value. Functions will not be executed by it self. It needs to be called. 


```javascript
function greet ( name ) {
    return "Hello" + name;
} 

greet( "Nur" );
```

******


### Allright finally the __FUN__ stuff

******

## Jquery


jQuery is a fast, small, and feature-rich JavaScript library.


******


### First Getting an element


with JavaScript

```javascript
document.getElementByClass(".first");
```

with jQuery

```javascript
$(".first");
```

******
### Changing Background Color 

```javascript
$(".first").css("background-color", "black");
```
******

### Changing  The Text Of The Paragraph

```javascript
$(".first p").text("HELLO WORLD");
```
******


### Toggle Effect

```javascript
$(".first").toggle();
```
******

### Document Ready

JavaScript is used to manipulate the document. So we want to wait until the document is loaded to run our javascript code. 

```javascript
$( document ).ready(function() {
    console.log( "ready!" );
});
```
******


### Document Ready

There are alot of times when you want to wait for the user to interact with the page to do something. 

```javascript
$( document ).ready(function() {
    $(".btn").click( function () {
        $(".first").slideUp();
    });
});
```

******

### Adding A New Element To The Document

```javascript
$( document ).ready(function() {
    $(".btn2").click( function () {
        $("<div><p>I am Inserted Here</p></div>").insertBefore(".buttons");
    });
});
```






