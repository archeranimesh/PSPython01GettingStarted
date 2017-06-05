# Chapter 03 | Functions, File, Yield and Lambda #

The topics which we will cover in this modules are

* Functions and its arguments.
* File Operations.
* Yield
* Lambda

## Functions and its arguments ##

* A function is a block of organized code, which does certain action.
* Each function should only perform only one task, and should not be a combination of unrelated task.
* Functions can be of two types.
    * Built-in function
        * like `len()`, `print()` etc.
    * User defined function.
* Function defination:-

````python
def function_name(arg1, arg2):
    statement 1
    statement 2
    return 
````
* `def` keyword signifies the start of the function, ends in `:`
* `function_name` is the name of the function which might be used to invoke the function.
* `arg1` and `arg2` are the data passed as arguments to the function.
    * A function can take, 0, 1 or multiple arguments.
* A function can `return` a value, to the caller.
* We can also have optional/default arguments.

### Function Arguments ###
* Arguments scope is local to the function.
* **Default/Optional Arguments**

```python
def function_name(name, student_id=335):
    return
```
* In the above example, `student_id` is the optional arguments, as it has a default values, so while calling `function_name('hello')` the `student_id` will be saved as `335`, in case we provide it, that value will be taken.

* **Named Argument**
    * We can also invoke arguments with the name.
```python
function_name(name="hello", student_id=45)
```
    * Once we invoke a function will named arguments, all the arguments to the right of this arguments have to be invoked with there name.


