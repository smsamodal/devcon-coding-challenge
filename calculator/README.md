# Calculator Interpreter

The challenge is to make an interactive interpreter with a number of different capabilities:

* It should be able to take a mathematical string and return the result of it
```
5 + 2
```
* It should be capable of assigning variables
```
x = 5 + 2
```
*  store the value for the variable for later use and return the value
* Use assigned variables instead of numbers
```
y = x * 2
```

* Variable names must start with a character `a-z` and can be continued by any alphanumeric character.

* All variables will be numerical (can be either floats or integers), feel free to support arbitrarily large numbers.

* The mathematical evaluator shall be capable of adding, subtracting, multiplying, dividing, exponents and handling nested parenthesis.
exponents will be using `^` as symbol.

The usual order of mathematics apply, so PEMDAS shall be applied in evaluations.

**PLEASE refrain from using your languages built in evaluators.**
