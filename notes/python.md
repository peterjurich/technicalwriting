# What is Python?
A dynamic, interpreted language
No declarations of variables, etc. source code makes it short and flexible
No need to remember syntax.

## Why use it?
Readable, easy to learn, free, cross platform, open source, large standard library

## What can it do?
Create web apps, use along software workflows, big data and complex math, rapid prototyping and production ready software dev.

## Need for Python?
Can work on many platforms, easy syntax for beginners, code can be executed as soon as its written (interpreted system) so prototyping is quick
Can be treated in a procedural way, an object-oriented way, or a functional way

## How different?
Designed for readability
Uses new lines to complete a command
Relies on indentation and white space

# Basic Syntax
Data input/output, basic syntax, practical examples

## Indentation
Code usually written in blocks. Indentation helps define blocks
Non-indented code is start of the block. Subsequent must be indented by one level.

### Rules for indenting
Do not indent first line of code.
The way you indent the second line must be the same way you indent subsequent lines.
It is best to use 1 tab or 4 white spaces
To indent automatically, use a colon
For example
`if 5>2:
    print ("Yes, five is greater than two")
print("No, five is not greater than two")`

# Comments
Explain the code to make it more readable.
Also prevents execution of test code.
Create comments by using pound sign (#) at the beginning, if single line of code
Alternatively, use """ at the beginning and end of an entire block.
Can put comments at the end of a line of code, too.
For example: print ("Hello world") #This is a printing code

# Variables
Act as a container for data values

## Rules for naming variables
Must start with letter or underscore.
CANNOT start with a number
Names are case sensative

You can give variables in the same line
For example: `x, y, z = "A", "B", "C"`
Can print as:
`print(x)
print(y)
print(z)`
or `print (x, y, z)`

### Multi-word names
Camel case: Each word except the first is capitalized
myVariableName

Pascal Case: Every word capitalized
MyVariableName

Snake Case: each word seperated by an underscore
my_variable_name

# Keywords
<img src="https://github.com/peterjurich/technicalwriting/blob/150d55f8ae2a968b948c4c63202039970a5d2a68/notes/Screenshot%202022-11-22%20at%2010.18.05%20AM.png" alt="A table of Python keywords" title="A table of Python keywords">

# Data types
Look up types by
x = 'string'
print(type(x))
Should pull up 'str'

Can change data types halfway through code

String: words in quotes
Int: Numbers
Float: Fraction, but will change to whole number if defined as float
Data structures: lists use [], tuples use (), sets use {}  
Range: x = range(5) will bull up (0,5)
bytes
complex: a number and letter combo like 6j

# Operators
## Arithmatical
+, -, *, /
% brings up the remainder
// converts fraction answer into a whole number (not not round up)
** It is x to the power of y, where x ** y

## Assignment
=
+= (add a number, i.e. x += 5) 
-= subtract a number
*= multiple by number
/= divide by a number
//= divide, but no fraction
%= for remainder
**= to the power of

## Comparison:
> greater than
< less than
>= greater than/equal to
<= less than/equal to
== is equal to
!= is not equal to

## Logical:
`x = 2
print (x>1 and x<5)` will bring up True

and: if both conditions are True, will print True

or: if at least 1 is True

not: include before print to do opposite
`x = 2
print (not (x>2 or x<5)
False`

# Conditions
Basic operators are ==, !=, <, >, <=, >=

## if
First conditional
`if a > b:`

## elif
Second conditional if first is false
`if b > a:`

## else 
If neither first nor second conditional are true. This has no condition attached
else:

## else if
If no second condition, you can simply go from if: to else:,

Can combine comparison and logical operators:
`a = 200
b = 100
c = 300
if a > b and c > a:
    print("Yes, both conditions are true.")`

## nested if
An if condition that is true only if another if is true
`x = 40
if x > 10:
    print("Greater than 10")
    if x > 20:
        print("Greater than 20")
        if x > 30:
            print("Greater than 30")`

## one line statement to define if
Can also write on same line, so `print ("True") if a < b else print ("False")`

Can do multiple conditionals on one line:
`a = 3
b = 30
print("True part of a > b") if a > b else print("True part of a == b") if a < b else print("B")`
Brings up `True part of a == b`

# Loops
Can use `continue` and `break` to determine whether the loop goes on.

## While loops
As long as something is true, loop will continue

## For loops

Defining properties in lists?

`list = ["car", "cycle", "bus"]
for a in list:
    print(a)`
will default a to all items in the list and pull up
`car
cycle
bus`

### Nested for loops
`fruits = ["apple", "banana", "grapes"]
color = ["red", "yellow", "green"]

for x in color:
    for y in fruits:
        print (x,y)`
        
# Data structures (arrays)
<img
src="https://github.com/peterjurich/technicalwriting/blob/64eb3af0f1a18113046d37c882b219f0a38678df/notes/Screenshot%202022-11-23%20at%201.14.50%20PM.png" alt="Data structures and their attributes" title="Data structures and their attributes">

## List
Is mutable: can add and delete items from list
To call specific spot in list, use something like `list[1]`
### List methods
<img
src="https://github.com/peterjurich/technicalwriting/blob/02040e7af037708c38662b718f92b4d9eaa819b3/notes/Screenshot%202022-11-23%20at%201.23.44%20PM.png" alt="List methods" title="List methods">

## Tuple
Immutable: cannot add or delete items
Can change a list to a tuple by changing brackets [] to parentheses ()
However, tuples are immutable, so cannot be appended, for example.
### Tuple methods
<img
src="https://github.com/peterjurich/technicalwriting/blob/d02a198164aac581bcb2d3e69e991243c21db8ca/notes/Tuple%20methods.png" alt="Tuple methods" title="Tuple methods">

## Set
Immutable and unordered, so they can appear in a different order everytime they are run
does not print duplicates, so `set2 = {"apple", "banana", "grapes", "grapes"}` will bring up `{'banana', 'grapes', 'apple'}`
Can still use `set.add()`, `set.pop()`, and `set.clear()`
### Set methods
<img
src="https://github.com/peterjurich/technicalwriting/blob/d02a198164aac581bcb2d3e69e991243c21db8ca/notes/Set%20methods.png" alt="Set methods" title="Set methods">

## Dictionary
Unordered, changeable, indexed
For example:
`dict = {
    "model":"Alto",
    "color":"red",
    "year":"2000"
}
print(dict)
print(dict["model"])
print(len(dict))
print(type(dict))`
### Dictionary methods
<img
src="https://github.com/peterjurich/technicalwriting/blob/d02a198164aac581bcb2d3e69e991243c21db8ca/notes/Dictionary%20methods.png" alt="Dictionary" title="Dictionary methods">
Keys method is unique to dictionaries, will return all values currently assigned to this item.
`x = dict.keys()
print(x)`
returns `dict_keys(['model', 'color', 'year'])`

Similarly,
`a = dict.values()
print(a)`
will return `dict_values(['Alto', 'red', '2000'])`

Printing `a = dict.listems()`, on the other hand, will return:
`dict_items([('model', 'Alto'), ('color', 'red'), ('year', '2000')])`

# Functions
`def` to define functions

`#Parameter goes in the parentheses of next line.
def first_function(full_name):
    #+ Arguments go into the following
    print(full_name + " Smith")`
    
The terms 'parameters' and 'argument' can be used similarly for how information is being passed to a function. From a function perspective, a parameter is like a variable to be declared.

An argument is a value that is sent to a function when it is called.

## Lists in functions:
`def function (*kid):
    print("The child in the middle is " + kid[1] + ".")
function("Anna", "Karen", "John")`
pulls up `The child in the middle is Karen.`

## For Loops in Functions
`def function(fruit):
    for a in fruit:
        print()
list = ["apple", "banana", "cherry"]
function(list)`
pulls up: `apple
banana
cherry`
## Return statements in Functions
`def myFunction(a):
    return 5 * a
print(myFunction(3))
print(myFunction(5))
print(myFunction(9))

15
25
45`

## Pass statements and functions
`def myFunction(a):
    pass`
Nothing happens

# Libraries and other resources
After installing a library to your computer, run `!pip install [name of file]`


