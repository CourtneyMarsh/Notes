# JAVASCRIPT

## Introduction

- **Remainder/Modulo %** operator returns the number that remains after the right-hand number divides into the left-hand number as many times as it evenly can
- **Null** is a primitive data type that represents the intentional absence of value
- **Numbers** are a primitive data type that include the set of all integers and floating point numbers
- **Single Line Comments** are created with two consecutive forward slashes **//**
- **.length** property of a string returns the number of characters that make up the string
- **Methods** return information about an object and are called by appending an instance with a period **.** the method name, and parantheses - Math **.random( );** normally as Math.random( );
- **Built-in Objects** contain methods that can be called by appending the object name with a period **.**, the method name, and a set of parantheses - **Math** .random( );
- **const** keyword - a constant variable is declared by using the keyword **const**.  However, a const variable cannot be reassigned because it is constant.  It must have an assignment.  Any attempt of re-assigning a **const** variable will result in a Javascript runtime error - const numberOfColumns =4;
- **Calling functions:** functions can be called or executed elsewhwere in code using parantheses following the function name.  When a function is called, the code inside its function body runs.  **Arguments** are values passed into a function when it is called
``` 
function sum(num1, num2) {
  return num1 + num2;
}

sum(2, 4); - this is calling the function
```
- **Function parameters:** inputs to functions are known as parameters when a function is declared or defined.  **Parameters** are used as variables inside the function body.  When the function is called, these parameters will have the value of whatever is passed in as arguments.  It is possible to define a function without parameters
**function sayHello(name) {
  return 'Hello, ${name}!';
  }**  
- **the parameter is name**
- The **let** keyword signals that the variable can be reassigned a different value - example below:
```
let meal = 'Enchiladas';
console.log(meal); // Output: Enchiladas
meal = 'Burrito';
console.log(meal); // Output: Burrito
```
- **If you’re trying to decide between which keyword to use, let or const, think about whether you’ll need to reassign the variable later on. If you do need to reassign the variable use let, otherwise, use const.**
- increment operator (++) and decrement operator (--)
- The increment operator will increase the value of the variable by 1. The decrement operator will decrease the value of the variable by 1
- **Concatenation in variable:** The + operator can be used to combine two string values even if those values are being stored in variables:
```
let myPet = 'armadillo';
console.log('I own a pet ' + myPet + '.');
// Output: 'I own a pet armadillo.'
```
- Insert, or interpolate, variables into strings using template literals. Check out the following example where a template literal is used to log strings together:
```
const myPet = 'armadillo';
console.log(`I own a pet ${myPet}.`);
// Output: I own a pet armadillo.
```
- a **template literal** is wrapped by backticks ` (this key is usually located on the top of your keyboard, left of the 1 key).
- Inside the **template literal,** you’ll see a placeholder, ${myPet}. The value of myPet is inserted into the template literal.
- When we **interpolate** `I own a pet ${myPet}.`, the output we print is the string: 'I own a pet armadillo.'
- The **typeof** operator checks the value to its right and returns, or passes back, a string of the data type.

**const unknown1 = 'foo';
console.log(typeof unknown1);** // Output: string
 
**const unknown2 = 10;
console.log(typeof unknown2);** // Output: number
 
**const unknown3 = true; 
console.log(typeof unknown3);** // Output: boolean

// value saved to kelvin will stay constant
```
const kelvin = 0;

// calculates celsius temp
let celsius = kelvin - 273;

// calculates fahrenheit temp
let fahrenheit = celsius * (9/5) + 32;

// rounds down fahrenheit temp
fahrenheit = Math.floor(fahrenheit);

console.log(`The temperature is ${fahrenheit} degrees Fahrenheit`);
```
## Conditionals

- A **conditional statement** checks a specific condition(s) and performs a task based on the condition(s).  **If-else decisions** can be modeled in code by creating conditional statements
- The if statement is composed of:

  -The **if** keyword followed by a set of parentheses () which is followed by a code block, or block statement, indicated by a set of curly braces {}.
  -Inside the parentheses (), a condition is provided that evaluates to true or false.
  -If the condition evaluates to true, the code inside the curly braces {} runs, or executes.
  -If the condition evaluates to false, the block won’t execute.

- An **else** statement must be paired with an if statement, and together they are referred to as an **if...else statement.**

- In the example above, the else statement:

  -Uses the else keyword following the code block of an if statement.
  -Has a code block that is wrapped by a set of curly braces {}.
  -The code inside the else statement code block will execute when the if statement’s condition evaluates to false.
  
- **if...else statements** allow us to automate solutions to yes-or-no questions, also known as binary decisions.
- When writing conditional statements, sometimes we need to use different types of operators to compare values. These operators are called **comparison operators.**
  -Less than: <
  -Greater than: >
  -Less than or equal to: <=
  -Greater than or equal to: >=
  -Is equal to: ===
  -Is not equal to: !==

- All **comparison statements** evaluate to either **true or false**
- There are three **logical operators:**

  -the and operator (&&)
  -the or operator (||)
  -the not operator, otherwise known as the bang operator (!)

- Because || or statements check the left-hand condition first, the variable defaultName will be assigned the actual value of username if it is truthy, and it will be assigned the value of 'Stranger' if username is falsy. This concept is also referred to as **short-circuit evaluation**
``` 
let username = '';
let defaultName = username || 'Stranger';
    console.log(defaultName); // Prints: Stranger
```
- **Ternary operator** to simplify an if...else statement:
 -EXAMPLE BELOW: 1st regular if ...else statement and 2nd ternary operator
```
let isNightTime = true;
 
  if (isNightTime) {
    console.log('Turn on the lights!');
  } else {
    console.log('Turn off the lights!');
  }
```
```
isNightTime ? console.log('Turn on the lights!') : console.log('Turn off the lights!');
```
- The **else if** statement allows for more than two possible outcomes. You can add as many else if statements as you’d like, to make more complex conditionals!
- A **switch statement** provides an alternative syntax that is easier to read and write than lots of **else if** statements. A switch statement looks like this:
```
let groceryItem = 'papaya';
 
switch (groceryItem) {
  case 'tomato':
    console.log('Tomatoes are $0.49');
    break;
  case 'lime':
    console.log('Limes are $1.49');
    break;
  case 'papaya':
    console.log('Papayas are $1.29');
    break;
  default:
    console.log('Invalid item');
    break;
}
 
// Prints 'Papayas are $1.29'
```
## Functions

- A **function** is a reusable block of code that groups together a sequence of statements to perform a specific task
- a **function declaration** binds a function to a name, or an **identifier.**
- A function declaration consists of:

  -The function keyword.
  -The name of the function, or its identifier, followed by parentheses.
  -A function body, or the block of statements required to perform a specific task, enclosed in the function’s curly brackets, { }.
- To **call a function** in your code, you type the function name followed by parentheses.
```
function getGreeting() {
    console.log('Hello, World!');
}

getGreeting();
```
- **Parameters** allow functions to accept input(s) and perform a task using the input(s).  We use parameters as placeholders for information that will be passed to the function when it is called.  **Parameters** are treated like variables within a function
- The values that are passed to the function when it is called are called **arguments.** **Arguments** can be passed to the function as values or variables.
- **Default parameters** allow parameters to have a predetermined value in case there is no argument passed into the function or if the argument is undefined when called.
```
function rectangleArea(width, height) {
    let area = width * height;
    return area;
  }
  console.log(rectangleArea(5, 7)) 
```
- To pass back information from the function call, we use a **return statement**
```
function monitorCount(rows, columns) {
  let grid = rows * columns;
  return grid;
}
const numOfMonitors = monitorCount(5, 4);
console.log(numOfMonitors);
```
- the return value of a function inside another function is **helper functions**
```
function monitorCount(rows, columns) {
  return rows * columns;
};
function costOfMonitors(rows, columns) {
  return monitorCount(rows, columns) * 200;
};
const totalCost = costOfMonitors(5, 4);
console.log(totalCost);
```
- Another way to define a function is to use a **function expression.** To define a function inside an expression, we can use the function keyword. In a **function expression,** the function name is usually omitted. A function with no name is called an **anonymous function.** A **function expression** is often stored in a variable in order to refer to it.
```
const calculateArea = function(width, height) {
  const area = width * height;
  return area;
};
```
- **Arrow functions** is a shorter way to write functions.  **Arrow functions** remove the need to type out the keyword function every time you need to create a function. **() =>**
```
const FUNCTION_NAME = (PARAMETERS) => {
    //Function Block
}

// How to invoke a function
FUNCTION_NAME(PARAMETER_VALUES_GO_HERE);
```
```
const plantNeedsWater = (day) => {
  if (day === 'Wednesday') {
    return true;
  } else {
    return false;
  }
};
```
```
greeting = () => {
  console.log('Hello, World!');
}

greeting();
```

## Scope

- A **block** is the code found inside a set of curly braces {}.
- **Scope** is the context in which our variables are declared.
- In **global scope,** variables are declared outside of blocks. These variables are called **global variables.**
- Because **global variables** are not bound inside a block, they can be accessed by any code in the program, including code in blocks.
- When a variable is defined inside a block, it is only accessible to the code within the curly braces {}. We say that variable has **block scope** because it is only accessible to the lines of code within that block.
- Variables that are declared with block scope are known as **local variables** because they are only available to the code that is part of the same block.
- **Scope pollution** is when we have too many global variables that exist in the global namespace, or when we reuse variables across different scopes.
- **Global namespace** is the space in our code that contains globally scoped information.

## Arrays

- **Arrays** are JavaScript’s way of making lists. **Arrays** can store any data types (including strings, numbers, and booleans).
```
let concepts = ['creating arrays', 'array structures', 'array manipulation'];
```
- An **array literal** creates an array by wrapping items in square brackets []. 
- Each content item inside an array is called an **element.**
- Each element in an array has a numbered position known as its **index.**  Arrays in JavaScript are zero-indexed, meaning the positions start counting from 0 rather than 1.
- **Update Elements:**
```
let seasons = ['Winter', 'Spring', 'Summer', 'Fall'];
 
seasons[3] = 'Autumn';
console.log(seasons); 
//Output: ['Winter', 'Spring', 'Summer', 'Autumn']
```
- Elements in an array declared with **const remain mutable.** Meaning that we can **change the contents of a const array,** but cannot reassign a new array or a different value.
- When we want to know how many elements are in an array, we can access the **.length** property.
- **.push()**, allows us to add items to the end of an array.
```
const itemTracker = ['item 0', 'item 1', 'item 2'];
 
itemTracker.push('item 3', 'item 4');
 
console.log(itemTracker); 
// Output: ['item 0', 'item 1', 'item 2', 'item 3', 'item 4'];
```
- **.pop()**, removes the last item of an array.
```
const newItemTracker = ['item 0', 'item 1', 'item 2'];
 
newItemTracker.pop('item2);
 
console.log(newItemTracker); 
// Output: [ 'item 0', 'item 1' ]
```
- Some arrays methods that are available to JavaScript developers include: .join(), .slice(), .splice(), .shift(), .unshift(), and .concat() 
- **Arrays & Functions example:**
```
const flowers = ['peony', 'daffodil', 'marigold'];
 
function addFlower(arr) {
  arr.push('lily');
}
 
addFlower(flowers);
 
console.log(flowers); // Output: ['peony', 'daffodil', 'marigold', 'lily']
```
- An array contains another array it is known as a **nested array.**
```
const nestedArr = [[1], [2, 3]];
```

## Loops