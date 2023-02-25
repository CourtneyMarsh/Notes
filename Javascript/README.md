# Eloquent Javascript Book

## Values, Types and Operators

 - **Values:** chunks of bits that represent pieces of information
 - **Strings** are used to represent text like "Float on the ocean" you can use single quotes, double quotes, or backticks to mark strings
 - 4 types of JS values: numbers, strings, Booleans, and undefined values

## Program Structure

 - **Expression:** a fragment of code that produces a value
 - A **program** is a list of statements
 - Binding or variables catch and hold values by using keywords
 - After a binding has been defined, its name can be used as an expression
 - The = operator can be used at any time on existing bindings to disconnect them from their current values and point them to a new one
 - **var** is short for variable and was used in the same was **let** is used now, probably won't use var very often
 - **const** stands for constant - it defines a constant binding which points at the same value for as long as it lives
 - **Environment:** the collection of bindings and their values that exist at a given time
 - **Function:** a piece of program wrapped in a value
 - Executing a function is called invoking, calling, or applying it
 - **Arguments:** values given to functions
 - When a function produces a value, it is said to **return** that value
 - **Conditional Execution:** when the program takes the proper branch based on the situation at hand (**if** keyword)
 - **counter = counter + 1** - easier format: **counter += 1** means it is counting upward
 - **counter = counter - 1** - easier format: **counter -= 1** means it is counting downward
 - **Writing a binding name with several words in it:**
 - fuzzylittleturtle
 - fuzzy_little_turtle
 - FuzzyLittleTurtle
 - fuzzyLittleTurtle - most commonly used
 - **Conditional:** if, else, and switch statements
 - **Looping:** while, do and for statments

## Functions

 - a function definition is a regular binding where the value of the binding is a function
 - **Scope:** part of the program in which the binding is visible
 - **Global:** bindings defined outside of any function or block
 - **Call Stack:** the place where the computer stores context
 - **Closure:** being able to reference a specific instance of a local bindng in an enclosing scope
 - **Recursive function:** a function that calls itself
 - **Pure Function:** is a specific kind of value-producing function that not only has side effects but also doesn't rely on side effects from other code - example: it doesn't read global bindings whose value might change

## Data Structures: Objects and Arrays

 - **Array:** stores a sequence of values
 - let listOfNumbers =[2, 3, 5, 7, 11];
 - console.log(listOfNumbers[2]);
 - 5
 - The first index of an array is zero
 - Two main ways to access **properties** in JS are with a dot and with square brackets: value.x or value[x] - access a property on value, but not necessarily the same property
 - mystring.length - gets the length of a string
 - Math.max - gets the maximum function
 - **Methods:** properties that contain functions - ex. .toUpperCase
 - .push adds values to the end of an array
 - .pop removes values the last value in an array
 - **Stack:** is a data structure that allows you to push values into it and pop them out again in the opposite order so that the thing that was 
 added last is removed first
 - Values of the type **object** are arbitrary collections of properties
 - **in** binary operator - when applied to a string and an object, tells you whether that object has a property within that name 
 - example of **in** console.log("left" in anObject)
 - Object.keys - finds out what properties an object has - it will return an array of strings
 - == operator compares objects by identity
 - **Correlation:** is a measure of dependence between statistical variables
 - **includes**: method that checks whether a given value exists in the array
 - **Classic JS Array Loops:**
 - for (let i = 0; i < JOURNAL.length; i++) {
 - let entry = JOURNAL[i];
 - }
 - **Modern JS Array Loops:**
 - for (let entry of JOURNAL) {
 - console.log(`${entry.events.length} events. `);
 - }
 - **Rest Parameter:** is bound to an array containing all further arguments - ex. function max(...numbers) the triple dot is the bind
 - **Serialize:** convert data into a flat description
 - **JSON:** popular sterilization format (pronounced "J Sawn") stands for JavaScript Object Notation.  It is widely used as a data storage and communication format on the web, even in languages other than JavaScript
 - All property names have to be surrounded by double quotes and only simple data expressions are allowed - no function calls, bindings, or anything that involves actual computation.  Comments are not allowed in JSON
 - **JSON.stringify** takes a JS value and returns a JSON-encoded string
 - **JSON.parse** takes such a string and converts it to the value it encodes


## Higher-Order Functions

- **Abstractions** hide details and give us the ability to talk about problems at a higher level
- **Higher-Order Functions:** functions that operate on other functions, either by taking them as arguments or by returning them
- **forEach** is used to loop over the elements in an array
- **filter** method returns a new array containing only the elements that pass the predicate function
- **map** transforms an array by putting each element through a function
- **reduce** to combine all the elements in an array into a single value
- **some** method tests whether any element matches a  given predicate function
- **findIndex** find the position of the first element that matches a predicate 