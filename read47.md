# Scopes in Python

There are 2 types of scopes in Python and in other programming languages in general

### Global Scope Variable(s)

![scope](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTQ1zWP63IFiXsZa9Y7zRSQ6m9Au4LAXjfFgQ&usqp=CAU)



-A variable declared outside of the function. This means that a global variable can be accessed inside or outside of the function.



```python
x = "global"

def foo():
    print("x inside:", x)


foo()
print("x outside:", x)
```

output will be: 
```
x inside: global
x outside: global
```

### Local Scope Variable(s)

-A variable declared inside the function's body or in the local scope is known as a local variable.

Example:

```python
def foo():
    y = "local"
    print(y)

foo()
```

output will be:
```
local
```

- Local (or function) scope is the code block or body of any Python function or lambda expression. This Python scope contains the names that you define inside the function. These names will only be visible from the code of the function. It’s created at function call, not at function definition, so you’ll have as many different local scopes as function calls. This is true even if you call the same function multiple times, or recursively. Each call will result in a new local scope being created.

- Enclosing (or nonlocal) scope is a special scope that only exists for nested functions. If the local scope is an inner or nested function, then the enclosing scope is the scope of the outer or enclosing function. This scope contains the names that you define in the enclosing function. The names in the enclosing scope are visible from the code of the inner and enclosing functions.
- What are Nonlocal Variables and where are they used ?

-Nonlocal variables are used in nested functions whose local scope is not defined. This means that the variable can be neither in the local nor the global scope.

Example:

```python
def outer():
    x = "local"

    def inner():
        nonlocal x
        x = "nonlocal"
        print("inner:", x)

    inner()
    print("outer:", x)

outer()
```


Output:
```
Output

inner: nonlocal
outer: nonlocal
```

- Global (or module) scope is the top-most scope in a Python program, script, or module. This Python scope contains all of the names that you define at the top level of a program or a module. Names in this Python scope are visible from everywhere in your code.

- Built-in scope is a special Python scope that’s created or loaded whenever you run a script or open an interactive session. This scope contains names such as keywords, functions, exceptions, and other attributes that are built into Python. Names in this Python scope are also available from everywhere in your code. It’s automatically loaded by Python when you run a program or script.
Random
There is a package in Python that allows the use of random numbers.

## Program Example 1
Generate a random number from 1 to 6.
 We will just generate a random number from 1 to 6 with the package like this:

>`import random`
>
>`print(random.randint(1,6))`
