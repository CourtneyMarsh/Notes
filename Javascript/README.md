# Javascript

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