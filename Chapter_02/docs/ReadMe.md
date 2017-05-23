# Chapter 02 | Data Types, Loops, Statements #

The topics we will cover in this one is modules are
* Data Types
* Flow Controls
* Loops & List
* Dictionaries
* Exceptions

## Data Types ##
Few important points for Python Data Types are:-
* Not many data types are inbuilt like other programming languages.
* It is a dynamically typed languages.
* Type hinting is provided in some latest version, but it is not mandatory.

Primimary data types in python are:-

* int
* float
* string
* boolean
* None.

Few other data types are
* Complex
* Bytes and ByteArrary.

Few complex data types are
* List
* Dictionaries
* Tuple
* Set
* FrozenSets

### int and float ###
* Integer denoted by `int` represent all integer values including +ive and -ive.
* Floats represent the decimal numbers.
* we can cast to each other type by using
    * `int()`
    * `float()` operators

### stings ###
* Strings represents text.
* In Python 3 the default is unicode strings.
* Strings can be denoted in these 3 ways
    * `' '` : can embed a '"' inside without escaping
    * `" "` : can embed a `'` inside without escaping
    * `''' '''` : This is for multiline
* Few important methods are
    * `.capatalize()`: Returns a string with its first Char capatalize.
    * `.replace(old, new)`: Replace a old string with new one.
    * `.isalpha()`: Returns true is all characters in the string are alphabets
    * `.isdigit()`: Returns true is all characters in the string are digits.
* String used with `.format()`
    * `"{0} is my {1}".format(name, machine)`
        * `{0}` will be replaced by `name`
        * `{1}` will be replaced by `machine`
    * `f"Hello {name} is {machine}"`

### Boolean and None ###
* Boolean has only 2 values
    * `True`
    * `False`
* Every data type in python can be evaluated to True and False.
* `None` is a special type were a variable is assigned no value.
* `None` has a special type as `NoneType`
* `None` always evaluates to `False`

## if Statement ##
* `if else` statement is used to decide the flow of the code.
* Simple if condition is shown by
    * `if number != 5:`
* if statement can use a combination of `and`, `or` keywords.
* We also have a Ternary if in Python
    * `"bigger" if a > b else "smaller"`

## List ##
* A list is denoted by
    * `[1,2,3,4]`
* A list can be accessed by index starting from 0
    * `a[0]`
* A list can also have `-`ive index
    * `a[-1]` returns last char.
* A list value can be changed by
    * `a[0] = 4`
* A list can be expanded by
    * `a.append(5)`
* A value can be checked to be present in the list by
    * `1 in a`
* We can also get the length of the list by
    * `len(a)`
* We can have hetrogenous elements in a list
* List slicing doest not modfiy the original list.

## Loops ##

In Python we mainly have 2 types of loops
    * `for`
    * `while`

* `for` loop looks like this.
    * `for name in student_names:`
    * `for x in range(1,5):`
    * `range(star, stop, step)`
* `while` loops look like this
    * `while x < 10:`
* Both `for` and `while` can be exited prematurely by using `break` 
* Both can skip a loop count by using `continue`

## Dictionary ##
* Dictionaries is a key,value pair, just like a json.
* empty Dictionary can be initialized by `a = {}`
* Nested Dictionary is also possible.
* We can also have list of Dictionary.
* Few Dictionary methods are:-
    * `student['name']` give the corresponding value.
    * `student.get("Not able to find", "Unknown")` return `Unknown`
    * `student.keys() ` return the list of keys
    * `student.values() ` returns the list of values.
    * `del student['names']` deletes the key value pair.

## Exceptions ##

* Exceptions cause the code to stop execution.
* A sample code blocks looks like this

```` 
try:
    last_name = student['last_name']
except KeyError:    # Case the KeyError and just print
    print("Error")
except TypeError as error:
    print(error)    # Prints some detailed error message.
````
* We can raise Exceptions by using `raise` keywords.
