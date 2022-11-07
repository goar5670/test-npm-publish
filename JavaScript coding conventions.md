# JavaScript Coding Conventions
Coding conventions are style guidelines for programming. They typically cover:

* Naming and declaration rules for variables and functions.
* Rules for the use of white space, indentation, and comments.
* Programming practices and principles.

Coding conventions secure quality, improve code readability, make code maintenance easier. They can be documented rules for teams to follow, or just be your individual coding practice.

## Variable Names
Use `camelCase` for identifier names (variables and functions). All names start with a letter.
```
firstName = "John";
lastName = "Doe";

price = 19.90;
tax = 0.20;

fullPrice = price + (price * tax);
```

## Spaces Around Operators
Always put spaces around operators `= + - * /`, and after commas:
```
let x = y + z;
const myArray = ["Volvo", "Saab", "Fiat"];
```

## Code Indentation
Always use 2 spaces for indentation of code blocks:
```
function toCelsius(fahrenheit) {
  return (5 / 9) * (fahrenheit - 32);
}
```
Do not use tabs (tabulators) for indentation. Different editors interpret tabs differently.

## Statement Rules
### General rules for simple statements:
Always end a simple statement with a semicolon.
```
const cars = ["Volvo", "Saab", "Fiat"];

const person = {
  firstName: "John",
  lastName: "Doe",
  age: 50,
  eyeColor: "blue"
};
```
### General rules for complex (compound) statements:
1. Put the opening bracket at the end of the first line.
2. Use one space before the opening bracket.
3. Put the closing bracket on a new line, without leading spaces.
4. Do not end a complex statement with a semicolon.

**Functions:**
```
function toCelsius(fahrenheit) {
  return (5 / 9) * (fahrenheit - 32);
}
```
**Loops:**
```
for (let i = 0; i < 5; i++) {
  x += i;
}
```
**Conditionals:**
```
if (time < 20) {
  greeting = "Good day";
} else {
  greeting = "Good evening";
}
```
## Object Rules
### General rules for object definitions:
1. Place the opening bracket on the same line as the object name.
2. Use colon plus one space between each property and its value.
3. Use quotes around string values, not around numeric values.
4. Do not add a comma after the last property-value pair.
5. Place the closing bracket on a new line, without leading spaces.
6. Always end an object definition with a semicolon.

**Example:**
```
const person = {
  firstName: "John",
  lastName: "Doe",
  age: 50,
  eyeColor: "blue"
};
```

Short objects can be written compressed, on one line, using spaces only between properties, like this:
```
const person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};
Line Length < 80
For readability, avoid lines longer than 80 characters.
```

If a JavaScript statement does not fit on one line, the best place to break it, is after an operator or a comma.

**Example:**
```
document.getElementById("demo").innerHTML =
"Hello Dolly.";
```

## Naming Conventions
Always use the same naming convention for all your code. For example:

Variable and function names written as `camelCase`
Global variables written in UPPERCASE (it's quite common)
Constants (like PI) written in UPPERCASE

## Loading JavaScript in HTML
Use simple syntax for loading external scripts (the type attribute is not necessary):
```
<script src="myscript.js"></script>
```
Accessing HTML Elements
A consequence of using "untidy" HTML styles, might result in JavaScript errors.

These two JavaScript statements will produce different results:
```
const obj = getElementById("Demo")
```
```
const obj = getElementById("demo")
```
If possible, use the same naming convention (as JavaScript) in HTML.