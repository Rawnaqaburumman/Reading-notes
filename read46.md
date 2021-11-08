# Python Scope & the LEGB Rule

![mir](https://miro.medium.com/max/409/0*hsE2OKgoLM3L6RL6.png)

The LEGB rule is a kind of name lookup procedure, which determines the order in which Python looks up names. For example, if you reference a given name, then Python will look that name up sequentially in the local, enclosing, global, and built-in scope. If the name exists, then you'll get the first occurrence of it.

### Understanding Scope
**Global scope**: The names that you define in this scope are available to all your code.

**Local scope**: The names that you define in this scope are only available or visible to the code within the scope.

## Global scope VS Local scope
+ **Global scope**: The names that you define in this scope are available to all your code.For example ,if you assign a value to a name outside of all functions—say, at the top level of a module—then that name will have a **global scope**.
```python
    result =0
>>> def cube(base):
...     result = base ** 3
...     print(f'The cube of {base} is: {result}')
...
>>> cube(30)
```
the scope for `result` variable is global ,this is means that it can be accessable from and where in the module 

+ **Local scope**: The names that you define in this scope are only available or visible to the code within the scope.For example, if you assign a value to a name inside a function, then that name will have a **local scope**

```python
>>> def cube(base):
...     result = base ** 3
...     print(f'The cube of {base} is: {result}')
...
>>> cube(30)
```
the scope for `base` variable is local ,this mean that it is not accessable from outside `cube `function 
