# Functions with Python

## Objectives

After this lesson students will be able to

* Write a Python function using the `def` keyword
* Include parameters and return statements in a Python function
* Describe the use of the `global` keyword
* Use named arguments and default values for arguments to a function

## The Basics

A function in Python has the same purpose as a function in other languages: To write reusable code that can be run at any time after the function as been written. If you're hopping over to Python after using JavaScript, you'll be relieved to hear that there is only really one way in Python to write functions! 

### `def` keyword

The `def` keyword is used much like the `function` keyword in JavaScript. It's used to declare or *define* the function. A function that prints "Hello world" in Python looks like this:

```py
def greeting():
  print('Hello world')
```

Notice the parts of the function:

* `def`: Keyword that indicates this is a function definition
* `greeting`: The name of the function (can be alphanumeric + underscores - see details below)
* `()`: An empty set of parentheses indicates that no data is expected to be passed into this function. Any parameters we want to define would go here
* `:`: The colon here is important. It indicated the end of the function signature and the start of the function's code
* `print('Hello world')`: This is the actual code that the function contains. 

#### Aside: Naming a Python function

Naming conventions for functions in Python follow many of the same guidelines as naming variables. Your function in Python should:

* Start with a letter or underscore
* Contain alphanumeric characters and underscores
* Be lowercase (use snake case: `like_this` instead of camel case or title case: `notLikeThis`)
* Not be a reserved keyword in Python (for example, no function can be named `def` or `if`)
* Be concise. Python functions can be any length within reason, but try to keep the names short and to the point. Try to make the function name informative about what it does. 

You can look into [more details here](https://www.dummies.com/programming/python/how-to-name-functions-in-python/) for more info about naming conventions in Python.

#### Aside: Stubbing a function

In JavaScript or another language, you may have done a process called "stubbing". This is a practice where you'd define functions, classes, routes, etc., with the intention of writing the actual code inside them later. It can be a useful practice when you want to plan out the overall structure of your program before getting into the line-by-line details of your code.

```js
function greeting() {
  // TODO: Write this code later
}
```

However, if you try to run this code in Python, you will get an error:

```py
def greeting():
  # TODO: This is a job for future me!
```

The error you get looks like this:

![Syntax Error](https://res.cloudinary.com/briezh/image/upload/c_scale,w_364/v1590000037/Screen_Shot_2020-05-20_at_11.39.42_AM_omq2ji.png)

In order to make a stub in Python what we want to use is the [pass keyword](https://res.cloudinary.com/briezh/image/upload/c_scale,w_364/v1590000037/Screen_Shot_2020-05-20_at_11.39.42_AM_omq2ji.png). As you might have expected given the name, the `pass` keyword does nothing. It's a placeholder, exactly what we want! Let's modify our Python stub above with the `pass` keyword to make the code functional again.

```py
def greeting():
  # TODO: This is a job for future me!
  pass # This let's the function have one line of code that just does nothing
```

## Parameters and Arguments

Parameters and arguments both describe data that goes into a function. Generally the subtle difference is that arguments are the bits of data you pass in, and parameters are the names that the function uses to understand the data that was passed in to it.

### A function with one parameter

Here's a function with one parameter - let's modify our greeting function from above to allow a person's name to be passed in.

```py
def greeting(name):
  print('Hello', name)
  
greeting('Erin')
greeting('Paolo')
greeting('Tanya')
```

We've called (executed) the function 3 times with different names. 
Expected Output:

```
Hello Erin
Hello Paolo
Hello Tanya
```

In the above example, `name` is the parameter. It's the data as defined within the function. Arguments on the other hand are the data that is passed in when the function is called. In this case, 'Erin', 'Paolo', and 'Tanya' are all arguments being passed into the greeting function.

### Multiple Parameters

STUB

### Named Arguments

STUB

### Default Values

STUB

## Global vs Local Variables

STUB