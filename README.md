# Python-2021

### Introduction to Python:

- `Python` is a programming language as well as a scripting language
- `Python` is Open Source and Free to use
- It can be used to run scripts, automate tasks, develop websites and softwares

## Basics of Python

### Installing Python:

- All `Linux` Operating Systems come pre-installed with the latest version of Python.
- For `Windows/Mac` Operating Systems you can download and install Python from the offical Python website: [here](https://www.python.org/downloads/release/python-3100/)
- To check if python has been installed correctly, just type `Python --version` in the CLI and it should show you the version of Python that you downloaded and installed.

### The `print()` function:

- The `print()` is a function in Python3 and is used to print statements to the console or the CLI.
- This is similar to the `echo` statement in Linux
- `print()` is a built-in function in Python
- Each `print()` function can accept `keyword arguments` and one of the arguments is `end=""`. This determines how Python should separate different print statements. By default `end="\n"` value is passed to the `print()` function. You can pass any character inside the `end=""`.
```
print ("This is a sample text",end="❤️")
print ("Separated by the heart emoji")
```
- Another `Keyword Argument` is `sep=""` and this determines how you want to separate the different words in the given string
```
print ("This is a sample text",end="❤️")
```

### Literals:

- `Literals` are values that are stored in the variables.
- There are different literals that are available in Python
  - Integer
  - Floating Point
  - Strings
  - Boolean
  
### Operators:

- Any operations that must be perfomed on a given values is called as `Operators`.
- The type of operation performed on the values depends on the type pf `Operators` used.
- Python supports the following `Operators`

|  **Operator**        | **Values**             |
| -------------------- | ---------------------- |
| Arithmetic operators | (+,-,*,/,//,%,**)      |
| Assignment operators | (=)                    |
| Comparison operators | (==, <, >, <=, >=, !=) |
| Logical operators    | (and or not)           |
| Identity operators   | (is, is not)           |
| Membership operators | (in, not in)           |
| Bitwise operators    | (&, \| , ~ ^)          |

### Variables:

- `Variables` are used to store values in Python
- They refer to a memory location and is also known as an identifier that are used to hold values.
- We do not have to specify the type of variable in Python as `Python is smart enough to get the variable type`.
- Variable names can be a group of both letters and digits, but they have to `begin with a letter or an underscore`
- More about Python Variables can be seen: [here](https://www.javatpoint.com/python-variables)

### The `input()` function:

- The `input()` function can be used to accept inputs from the user.
- Similar to the `print()` function it can accept arguments and expects an user input in return when it is executed.
- All values accepted from the `input()` are `String` values even if the user inputs an integer value.
- If you want to convert the Value given by the user into a numberic data then you must `typecast` the value.
  - int()
  - float()
  - str()

### The `str()` function:

- You can use `+` to concatenate two strings
- You can use `*` to repeat the same string multiple times
- The `str()` function can be used to typecast a integer into a String value.

## Conditional Statements:

### if, else and elif Statements:

- **if Statement** - The **'if'** statement is used to check if the variable matches a particular value or not. If the expression evaluates to **'True'** then the block of code under the **'if'** statement is executed. 

```
if <condition>:
    print ("The condition is true")
```

- **else Statement** - The **else** statement is used if you want to have more than one condition to be checked. If the condition of **if** evaluates to **'True'** then the block of code under the **'if'** statement is executed. Otherwise the block of code under the **'else'** statement is executed. 

```
if <condition>:
    print ("The condition is true")
else:
    print ("This block of code will be executed")
```

- **elif Statement** - The **elif** statement is used when you need to have multiple i.e. more than two conditions to be checked. The block of code that evaluates to **'True'** is executed.


```
if <condition>:
    print ("The condition is true and loop will exit")
elif:
    print ("This block of code will be executed and exit the loop")
else:
    print ("This block of code will be executed")
```

## Loops in Python:

### While Loops:

- **While Loops** - The **'While'** loops statements are used when you want to run a block of code for a specified number of times or if you want to run a block of code until the condition of the statement evaluates to **'False'**

```
while <expression>:
    print ("Will be executed until expression evalues to false")    
```

- The **'While'** loop statements are **'Entry Check Loops'** meaning that the condition is checked before entering the loop and exits when the condition is not satisfied. i.e. The Loop will not run even once if the condition is not satisfied.

- **Break Statements** -  The **Break Statements** are used when you want to exit/break a block of code and resumes execution at the next statement    

```
for <expression>:
    if <condition>:
        break
    print("Exiting the If Condition")
print("Exiting the For Loop")
```

- **Continue Statement** - The **Continue Statements** are used when you want to return the control to the beginning of the while loop. The continue statement rejects all the remaining statements in the current iteration of the loop and moves the control back to the top of the loop. The continue statement can be used in both while and for loops.

```
for <expression>:
    if <condition>:
        continue
    print("Exitig the If Condition")
print("Exiting the For Loop")
```

### For Loops:

- **For Loops** - The **For** loops can be used when you know how many number of times you want to run the loop. The **While** loop can be used to achieve the same results, but the **For** loop is the most defined way to code when you know how many times you want to run the loop.
```

for val in sequence:
    loop body
```

## Boolean Expressions and Operators:

- **Boolean Expressions** - Boolean Expressions can contain either 'True' or 'False'.
- **Boolean Operators** - Boolean Operators are expressions that can evaluate to a Boolean Value i.e. 'True' or 'False'. The Boolean Operators or the Logical Operators are **And, Or and Not**

### The 'OR' operator Truth Table:

| Expression | Evaluates to  |
|--|--|
| True or True | True  |
|True or False | True |
|False or True| True|
|False or False| False|

### The 'AND' operator Truth Table:

| Expression | Evaluates to  |
|--|--|
|True and True | True|
|True and False | False|
|False and True | False|
|False and False| False|

### The 'NOT' operator Truth Table:

| Expression | Evaluates to  |
|--|--|
|not True | False  |
|not False | True |

## Lists in Python:

- `List` are used to store multiple items in a Single Variable
- `List` are created using square brackets `[]`
- They are ordered, mutable and allow duplicate values.
- The items in a `List` are indexed, the first item has the index `[0]`
- The last item in the `List` has the index `[-1]`
- If you add a new item to the list, the item will be added at the end of the list.
- To determine the number of items in a list, use the `len()` function
```
thislist = ["apple", "banana", "cherry"]
print(len(thislist))
```
- The `del` keyword can be used to delete the item at a given index
```
del item[2]
```
- You can use the built-in list methods to manipulate the existing list
- Some of the built-in list methods are `list.append()` and `list.insert()`
- `list.append()` can be used to add a new item to the end of the list.
- `list.insert()` can be used to add a new item at the mentioned index.
```
list.insert(2,"new_value") #insert new_value at index 2
```
- You can swap the values in the given list using the following snippet easily, without having to use a temp/third variable.
```
items[0], items[1] = items[1], items[0]
```
- `list.sort()` can be used to sort the list in the ascending or the descending order. Default is `ascending`
- `list.reverse()` can be used to reverse the items in a given list.
- `list.pop(i)` can be used to remove the item from a given index
- The items in a list can be sliced.
```
print (items[1:]) # Will print all items from index[1] till end of the list

print (items[:3]) # Will print all items from index 0 to index[2] "(3-1)"

```

## Functions in Python:

### Built-in Functions:

- Python has a large number of Built-in functions that can support the users to achieve the most commonly used or the perform the common tasks. The functionalities of these Built-in functions are pre-defined and can be used to perform several functions. Some of the commonly used Built-in functions are **print(), int(), len(), abs(), append() etc.**

- The **import** statement can be used to import new modules and get access to new functions
* `import <module_name>` -  But you have to use the function in the following way `module_name.function_name()`

* `from <module_name> import function_name` - Then you can invoke the function without having to mention the module name just by `function_name()`

### User Defined Functions:

- Users can write their own functions in Python using the `def function_name()` statement and execute the function by just calling the `function_name()` where you want to execute it. 
```
def input_number():
    return int(input("Enter a number:"))
```
- Users should consider defining functions where ever necessary where they are finding themselves using the same block of code again and again in order to prevent duplicating. 

- Functions also provide better readability, better run-time, and in-case you want to change what the code does, you just have to change it in the function rather than multiple lines of code.

- You can also pass parameters to your functions and such functions are called as **Parameterized Functions** and can accept arguments depending on the number of parameters the function accepts.