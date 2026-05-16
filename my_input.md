In Python, functions are blocks of code that can be executed multiple times from different parts of your program.
They serve several purposes:

1. **Modularity**: Functions help keep your code organized by breaking it down into smaller, more manageable
pieces.

2. **Reusability**: Functions enable you to reuse code in different contexts without having to duplicate the same
code over and over.

3. **Readability**: When functions are named correctly, they clearly indicate what a block of code does, making
your program easier to understand.

Here's a basic example of defining and calling a function in Python:

```python
def greet(name):
    print(f"Hello, {name}!")
greet("John")
```

**Defining a Function:**

1. The `def` keyword is used to define a function.
2. The name of the function follows `def`, e.g., `greet`.
3. Inside the parentheses after the function's name, you specify the parameters (or arguments) that can be passed
into it.

**Parameters in Python Functions:**

1. Parameters are values passed to functions when they're called.
2. They must match the types of variables defined inside the function for them to work correctly.
3. You can have multiple parameters by separating them with commas within the parentheses.
4. Each parameter has a type (e.g., `int`, `str`) if you specify one, or is left unspecified for dynamic typing.
5. Some common types are:
   - `int` for integers
   - `str` for strings
   - `bool` for boolean values (True/False)
   - `float` for floating-point numbers

**Function Parameters Example:**

```python
def add(a, b):
    return a + b
result = add(5, 7) # Output: 12
```

In this example:

- `a` and `b` are the parameters of the function.
- The type of these variables is inferred by Python to be integers since they're being used in an arithmetic
operation.
- When calling the `add` function with arguments `5` and `7`, it returns their sum, which we store in the variable
`result`.

**Function Default Parameters:**

You can also define functions that use default values for parameters. Here's how:

```python
def greet(name="John", age=30):
    print(f"Hello, {name}. Your age is {age}!")
greet() # Hello, John. Your age is 30!
greet("Alice") # Hello, Alice. Your age is 30!
```

In this example:

- The `name` parameter defaults to `"John"` and the `age` parameter defaults to `30`.
- If you call the function without specifying these values (as in `greet()`), they're used as their default
values.
- When you specify them, those become their actual values.