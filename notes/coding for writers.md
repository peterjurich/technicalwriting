Many programming languages like Java, JavaScript, and C# evolved from C, so they're "C-style." Others, like Python and Ruby, did not, but the only difference is in syntax.

5:10
1. Introduction to Programming
1. Introduction
Two kinds of languages: programming and scripting.

Programming: designed to minimize errors, but harder to program

Scripting (like JavaScript): easier to program, errors not caught as early

5:53
1. Introduction to Programming
1. Introduction
Application Programming Interface (API) is a protocol for communicating with a comp

Software Development Kit (SDK) is API + docu + tools that make it easy to perform some functionality

Web API is comming over the web

Platform APIs is comming with programming language; sometimes called SDKs

7:40
1. Introduction to Programming
1. Introduction
JS uses less code than Java, so it doesn't catch mistakes as easily. Used mostly for websites, and learning JS will teach some common prog concepts

1:09
1. Introduction to Programming
2. What is Programming?
Programs are organized into functions, which all has a series of steps. Functions can call other functions and can have data passed in/out.

2:41
1. Introduction to Programming
2. What is Programming?
An instruction can span more than one line. In C-style languages, you end an instruction with a semicolon

3:28
1. Introduction to Programming
2. What is Programming?
Even though the kind of space btw words doesn't matter, making code readable is helpful.

3:57
1. Introduction to Programming
2. What is Programming?
HTML and JavaScript (JS) work in tandem:

HTML defines look and layout

JS defines interactivity (like clicking a button or loading data)

5:16
1. Introduction to Programming
2. What is Programming?
As a TW, I'll be writing docu for SDK libraries (code to do certain functionality)

1:11
2. Programming with data
4. Data Types
Common data types:

String (text) (surrounded by double quotes (") in C-style languages)

Use single quote (') for single characters

Number

Boolean (T or F statement)

Complex data types

User interface elements, like buttons

Custom data "objects"

2:01
2. Programming with data
4. Data Types
String concatenation: joining two strings

"Hello" + "World" = "HelloWorld"

2:28
2. Programming with data
4. Data Types
\n = new line

\t = tab

3:16
2. Programming with data
4. Data Types
If string has quotation marks, use \" for the marks you want to show up

"Call me \"Peter\"" = Call me "Peter"

3:27
2. Programming with data
4. Data Types
If string has a backslash, then use \\

3:42
2. Programming with data
4. Data Types
Using a backslash in code is called "escaping"

4:20
2. Programming with data
4. Data Types
In many C-style languages, integers (whole numbers) and decimals are treated differently, but in JS, they are just considered the number data type.

5:29
2. Programming with data
4. Data Types
Some integers are written as hexadecimal, which are base 16 (0-9, A-F)

5:42
2. Programming with data
4. Data Types
For large numbers, e = "times the power of 10"

7:11
2. Programming with data
4. Data Types
Objects have other data types inside of them, like user interface elements and structured data.

8:00
2. Programming with data
4. Data Types
In JS, everything can be set to null, or nothing. Data is typically set to null to indicate the value hasn't been set yet or the program was not successful in setting a value.

1:17
2. Programming with data
6. HTML and JavaScript
HTML is static and doesn't react to outside actions.

3:20
2. Programming with data
6. HTML and JavaScript
3 ways to add JS into HTML:

put code in <script> tag

put it in a separate file: <script src="myFile.js"></script>

Put JS in-line.

5:16
2. Programming with data
6. HTML and JavaScript
Periods are used in object-oriented programming to indicate that something belongs to something else.

demoParagraph.innerHTML = "New text";



6:00
2. Programming with data
6. HTML and JavaScript
Since errors in code are not always obvious, opening the JS console for your browser will help you decode the error (Cmnd + Optn + J on Chrome)

0:11
2. Programming with data
8. Variables
Variables: how computer program store/retrieve data. They have:

name

data type

tell a computer to reserve memory for a variable

Statically typed: variable cannot change its type

Dynamically typed (like JS): variable can change type at any time

In JS, declare variable with var: var age; var userName; var isChecked

value

Assigned to variable w/ = age = 25

Or declare var and assign value at once: var age = 25



5:13
2. Programming with data
8. Variables
Constant: you can declare a var a constant so you get an error if the prog accidentally tries to change it: const companyName = 5

Put constants at the top of your code so you can change them if need be.

Common constants:

Codes

Error messages

Display information

6:16
2. Programming with data
8. Variables
Constants need docu for:

Name

Type

Value

Use: need to get this info from code comments or dev team

8:10
2. Programming with data
8. Variables
For documenting constants, this guy prefers a table with columns for name, description, type, and value.

0:06
2. Programming with data
10. Operators
Operators: symbols that transfer one or two values into another value

Two types of operators:

Binary: has a value before and after it. 1 + 2

Unary: has a value after it. -10

1:25
2. Programming with data
10. Operators
Several binary operators: +, -, *, /, % (divides two numbers and takes the remainder

One common unary operator: negative symbol

2:40
2. Programming with data
10. Operators
% (mod)

To find the last digit of x: x % 10

Zero if x is a leap year: x % 4

If a % b = 0, then a is divisible by b

One if x is an odd number: x % 2

2:57
2. Programming with data
10. Operators
Comparative operators: several binary operators that compare values

* == Equal to
* != Not equal to
* > Greater than
* < Less than
* >= Greater than or equal to
* <= Less than or equal to

3:48
2. Programming with data
10. Operators
Operation order

Parentheses first

If order of ops is not what you want, then use () to  force certain operations first

Unary minus sign

*, /, % (L to R)

+, - (L to R)

Comparisons: <, <=, etc.

5:39
2. Programming with data
10. Operators
Equals is == because = is already taken by assignment of values

6:13
2. Programming with data
10. Operators
Assignment shortcuts in C-style languages:

* ++ Add one, so x++ is the same as x = x + 1
* -- Subtract one
* += Add something
* -= Subtract something
* *= Multiply something, or x = x * 3
* /= Divide something
* %= Mod something

String operators
* + Adds two strings
* == Compares two strings to see if equal
* =! Compares two strings to see if not equal
                   
7:00
2. Programming with data
10. Operators
One binary string operator: the + sign, which concatenates two strings

Two comparison string operators: == (equal to) and != (not equal to)

8:09
2. Programming with data
10. Operators
Boolean operators:

* && (And) where both values need to be true for it to return true
* || (Or) where one value needs to be true for it to return true
* ! (Not)
                   
10:00
2. Programming with data
10. Operators
One unary Boolean operator: ! (Not)

This switch true values to false and false values to true

!true == false

0:49
3. Functions, Conditionals, and Loops
12. Functions
Functions are groups of code used to:

React to events

ex. user event like a button click

server event like a request for data

Make code easier to understand if it is broken up into smaller chunks

Reuse code so that it's not duplicated

If writing code in two place, better to turn that code into a function that you can call twice -- this way, if you need to make a change, you only need to change it once.

2:03
3. Functions, Conditionals, and Loops
12. Functions
You can pass data -- any number of values separated by commas --a into functions using parentheses. These are called parameters

2:39
3. Functions, Conditionals, and Loops
12. Functions
Creating a function includes:

Name

Parameters

What is returned

function squareRoot(x) {
return Math.pow(x, 0.5);

}

3:02
3. Functions, Conditionals, and Loops
12. Functions
Use function by calling it, then putting in parentheses the data you want passed. When you create a function, the parameters act like local variables

5:32
3. Functions, Conditionals, and Loops
12. Functions
When you are done with a function, you can return it by typing "return" and the computer considers the function done.

If function doesn't return a value:

Simply don't have a return line

Use return with nothing following it

6:00
3. Functions, Conditionals, and Loops
12. Functions
Two types of variables:

Local

Declared in a function and exists only in that function

Two functions can have variables w/the same name, but vars are still different

Global

Declared outside of the function

Changes made to var in one function affect its use in other functions

Good practice to declare these at the top of your code

8:11
3. Functions, Conditionals, and Loops
12. Functions
It's good to use local variables as much as possible the more complex your programs become bc it's much easier to keep track of what's happening w/them

0:50
3. Functions, Conditionals, and Loops
14. Documenting Functions
Function, or method, docu needs an explanation for:

Why someone would call a function

How someone would call a function

Primary will need to write about:

Description

Parameters

Return value

3:31
3. Functions, Conditionals, and Loops
14. Documenting Functions
Should start with a one-sentence description that begins w/a verb in present tense

3:57
3. Functions, Conditionals, and Loops
14. Documenting Functions
Follow description w/any further notes about the function

After these remarks, go to Parameters. You should contain the name, data type, and description of each parameter using short sentence fragments.

Ex. mode

Type: string

Camera mode

4:45
3. Functions, Conditionals, and Loops
14. Documenting Functions
Include return value with data type and description

0:35
3. Functions, Conditionals, and Loops
16. Conditionals
Conditionals, or if-then statements, execute a block of code if a statement is true.

If statements can be nested in other if statements, called nested ifs.

Else statements execute code if the statement is not true. The blocks of code are always contained in curly brackets

Else-if statements are executed if expression is false, but also checks if another expression is true.

Switch statements are easier ways to design the above.



1:10
3. Functions, Conditionals, and Loops
18. Making Your Code Readable
Comments in code is just for people to read. All C-style languages use: /* ... */

Where everything inside those is ignored by the computer.

But more common  to use double slashes: // ... //

2:06
3. Functions, Conditionals, and Loops
18. Making Your Code Readable
Devs rarely use enough comments

If you include them

Write in complete sentences

Put them at the beginning of each file or each function, or inside functions before there is a lot of complexity

Occasionally at the end of the line if some extra info will help

0:40
3. Functions, Conditionals, and Loops
20. Loops
A loop has several required parts:

Starting value, so j = 0

Continuation test, so j < 10. If this Boolean is true, we keep going

An increment, or j = j + 1

Repeats these things until j = 10 and therefore, Boolean is no longer true.

While loop: a code is repeated as long as a Boolean expression, or condition, is true

while (condition) {

  code block to be executed

}

For loop: Code is repeated while a value of the variable is changed

If going to use a variable only in a loop, then declare the var in the loop:

var numberString = ""
for (var i = 0; i <4; i++) {
numberString += i + " ";

9:31
3. Functions, Conditionals, and Loops
20. Loops
Most common for loop is:

for (i = 0; i < totalNumber; i++) {

7:03
4. More Advanced Concepts
22. Advanced Function Documentation
After documenting one function, might be helpful to have a See Also section with links to related functions

7:32
4. More Advanced Concepts
22. Advanced Function Documentation
Ideal to include 3-10 lines of sample code. Should be kept in sync with any code updates.

Should be meaningful and not just a line that calls the code

0:55
4. More Advanced Concepts
24. Introduction to Object Oriented Programming
Object-oriented programming (OOP) is a way to organize code in large software projects with thousands of variables and functions.

Classes: a group of relate vars and funcs

contains fields/properties (vars), and methods (funcs)

Members: methods and properties together

You can instantiate an object in that class type

3:16
4. More Advanced Concepts
24. Introduction to Object Oriented Programming
To set a property, put on left side of =. To get it, put it on the right side
textbox.size = 20;
var maxCharacters = textbox.size;

Use periods to string more properties together. ex:  page.textbox.size

5:48
4. More Advanced Concepts
24. Introduction to Object Oriented Programming
The vast majority of SDKs and object-oriented, so you're more than likely going to be documenting OOP in SDKs.

Classes need a one-sentence description often starting with "Represents..."

Properties are docu'd like constants; methods like functions.

2:41
4. More Advanced Concepts
25. Programming Languages
C++ is C, but object-oriented. Still just as fast, so many video games written in C++

Java: removed a lot of C++ complexities. Used primarily for Android and back-end (server) software; generally taught as first language

JavaScript was devved for web bc Java was too restrictive; OOP, dynamic, used for mobile apps

Python designed to be simple, readable, used for web apps and manipulating data/files

Ruby: btw Python and Java, makes mobile app dev easier

SQL is purely data language

0:47
5. Advanced Capabilities
26. Collections
Collections hold multiple pieces of data, as opposed to variables, which only hold one.

Two most common colls are:

arrays: organize data into a list

have a size (how many in list); and order (which comes first, second, etc.)

represented in JS by square brackets, where each value is separated by commas

Common JS array methods/properties

lengths (how many); indexOf (searches for object & returns position); push (adds new element to end of array & returns new length); reverse (reverses or of array elements); sort (sorts elements

It's very common to loop through all values of an array using a for loop

5:29
5. Advanced Capabilities
26. Collections
dictionaries (or hashtables): collection of data keys and values, where you use the key to look up the value.

Like in a dictionary where you use the word to look up the meaning.

Ex: Dictionary of U.S. regions (keys) and number of states (values). "Midwest": 10

In JS, objects and classes are the same and enclosed in { }

Keys and vals separated by :, pairs by ,

Keys and vals can be any data ty

0:07
5. Advanced Capabilities
28. Enumerations
Enumerations: special data type that holds discreet states; can only have values specified in a list

First: define the enum by giving it a name; then you use it with name.value



1:49
5. Advanced Capabilities
28. Enumerations
How to use in Java:

First declare, usually all caps
enum trafficLight {RED, YELLOW, GREEN};

Then use it
if (currentLight ==  TrafficLight.RED) {



2:53
5. Advanced Capabilities
28. Enumerations
JS does not have enums, but you can create something like it with constants:

const TrafficLight = {
RED: 0
YELLOW: 1
GREEN: 2
};
Use it similarly:
if (currentLight == TrafficLightd.RED) {

3:30
5. Advanced Capabilities
28. Enumerations
Docu enums w/

a short description

a v short desc of each value

the numeric value, only if important

Typically in table

0:07
5. Advanced Capabilities
30. Libraries
Libraries (or modules in JS) are a self-contained set of code that provides functionality. They add capability to your code.

They are imported into code, and are smaller/faster parts of a whole.

To docu, you need:

class

method

prop

const

enum

Why use this library?

How to get started?



1:54
5. Advanced Capabilities
30. Libraries
Easiest way to use JS module is <script> tag, then add a type and source ("src")

<script type="application/javascript"
     src="myModule.js"></script>
Then you can use any func or var in that module

Other way is using the import keyword, which allows you to bring in part of the module, and add a name to all funcs and vars in the module, but this does not work w/all implimentations of JS

3:06
5. Advanced Capabilities
30. Libraries
Libraries can be located locally or on the web. JS can read both.

0:54
5. Advanced Capabilities
32. Automated Documentation Generation
Automated Documentation Generation

Documentation is included in code as special comments

If code changes, docu right next to it

Runs a program that runs all comments and generates HTML docu

2:17
5. Advanced Capabilities
32. Automated Documentation Generation
Critical for comment block to be right above the func

 /**
* Creates a new event for the specified calendar.
* @param calendarId {Number} The ID of the calendar
* @return {Number} The ID of the new event
*/
function newEvent(calendar Id) { 
