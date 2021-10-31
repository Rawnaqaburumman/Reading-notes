# Testing and Modules:
### What is Unit tests: 
Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code
![unit test](https://cdn.guru99.com/images/unit-testing.png)

## Important aspects about the unit test:
##### test name: 
- We need to be descriptive about it and to say what is expected and what we are testing
- test file name should follow the same name of module name

### The cycle of test is made by three steps:
- Write a unit test and make it fail
-  Write the feature and make the test pass!
-  Refactor the code
The greatest advantage about TDD is to craft the software design first .Your code will be more reliable: after a change you can run your tests and be in peace
Beginning may be hard — and that’s fine. You just need to practice!

### What does the if __name__ == “__main__”: do?
 when python interpreter  run the module (the source file) as the main program, it sets the special __name__ variable to have a value “__main__”.
If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable. 

### Advantages : 
- If you import this script as a module in another script, the __name__ is set to the name of the script/module.
- if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported.
