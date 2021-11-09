

## List Comprehensions in Python

### **Create a List with range()**

- Let’s start by creating a list of numbers using Python list comprehensions. We’ll take advantage of Python’s **range()** method as a way to create a list of digits.

**Example 1: Creating a list with list comprehensions**

```python
# construct a basic list using range() and list comprehensions
# syntax
# [ expression for item in list ]
digits = [x for x in range(10)]

print(digits)

Output____

[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```
![](https://miro.medium.com/max/1400/1*uFMINpEzlskS-QkLfYeuiw.png)
# List Comprehensions in Python
It consists of brackets containing an expression followed by a for clause, then zero or more for or if clauses. The expressions can be anything, meaning you can put in all kinds of objects in lists.
The result will be a new list resulting from evaluating the expression in the context of the for and if clauses which follow it.
The list comprehension always returns a result list.
If you used to do it like this:
new_list = []
for i in old_list:
    if filter(i):
        new_list.append(expressions(i))
You can obtain the same thing using list comprehension. Notice the append method has vanished!
new_list = [expression(i) for i in old_list if filter(i)]
Syntax
The list comprehension starts with a ‘[‘ and ‘]’, square brackets, to help you remember that the result is going to be a list.

The basic syntax uses square brackets

[ expression for item in list if conditional ]
This is equivalent to:

for item in list:
    if conditional:
        expression
Let’s break this down and see what it does.
new_list = [expression(i) for i in old_list if filter(i)]
new_list The new list (result).
