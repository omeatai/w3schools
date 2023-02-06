# w3schools

w3schools Tutorials

## Tutorial

---

### [1-PYTHON COURSE - W3SCHOOLS](#)

+INTRODUCTION

<details>
  <summary>1. Python Introduction</summary>

Python is a popular programming language. It was created by Guido van Rossum, and released in 1991.

It is used for:

- web development (server-side),
- software development,
- mathematics,
- system scripting.

What can Python do?

- Python can be used on a server to create web applications.
- Python can be used alongside software to create workflows.
- Python can connect to database systems. It can also read and modify files.
- Python can be used to handle big data and perform complex mathematics.
- Python can be used for rapid prototyping, or for production-ready software development.

```py
print("Hello, World!")
```

```py
# Hello, World!
```

```py
x = "Python is awesome"
print(x)
```

```py
# Python is awesome
```

```py
x = "Python"
y = "is"
z = "awesome"
print(x, y, z)
```

```py
# Python is awesome
```

```py
x = "Python "
y = "is "
z = "awesome"
print(x + y + z)
```

In the print() function, when you try to combine a string and a number with the + operator, Python will give you an error.

```py
# Python is awesome
```

check Python version:

```bs
python --version
python -V
```

Run Python File:

```bs
python index.py
```

Run Python Shell:

```bs
python
```

```bs
Python 3.9.12 (main, Apr  5 2022, 01:53:17)
[Clang 12.0.0 ] :: Anaconda, Inc. on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> print("Hello")
Hello
>>> exit()
%
```

</details>

<details>
  <summary>2. Python Comments </summary>

- Python has commenting capability for the purpose of in-code documentation.

- Comments start with a #, and Python will render the rest of the line as a comment.

- Comments can be used to explain Python code.

- Comments can be used to make the code more readable.

- Comments can be used to prevent execution when testing code.

- Comments can be placed at the end of a line, and Python will ignore the rest of the line.

- A comment does not have to be text that explains the code, it can also be used to prevent Python from executing code.

- Python does not really have a syntax for multiline comments.

- To add a multiline comment you could insert a # for each line.

- Since Python will ignore string literals that are not assigned to a variable, you can add a multiline string (triple quotes) in your code, and place your comment inside it.

```py
#This is a comment.
print("Hello, World!")
```

```py
print("Hello, World!") #This is a comment
```

```py
#print("Hello, World!")
print("Cheers, Mate!")
```

```py
#This is a comment
#written in
#more than just one line
print("Hello, World!")
```

```py
"""
This is a comment
written in
more than just one line
"""
print("Hello, World!")
```

</details>

<details>
  <summary>3. Python Variables </summary>

- Python has no command for declaring a variable.

- A variable is created the moment you first assign a value to it.

- Variable names are case-sensitive.

- A variable can have a short name (like x and y) or a more descriptive name (age, carname, total\*volume).

Rules for Python variables:

- A variable name must start with a letter or the underscore character
- A variable name cannot start with a number
- A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and \* )
- Variable names are case-sensitive (age, Age and AGE are three different variables)

Legal variable names:

```py
myvar = "John"
my_var = "John"
_my_var = "John"
myVar = "John"
MYVAR = "John"
myvar2 = "John"
```

- Camel Case = myVariableName
- Pascal Case = MyVariableName
- Snake Case = my_variable_name

```py
x = 5
y = "John"
print(x)
print(y)
```

```py
# 5
# John
```

```py
x = 4       # x is of type int
x = "Sally" # x is now of type str
print(x)
```

```py
# Sally
```

```py
a = 4
A = "Sally"
#A will not overwrite a
```

Many Values to Multiple Variables-

- Python allows you to assign values to multiple variables in one line:

```py
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)
```

```py
# Orange
# Banana
# Cherry
```

One Value to Multiple Variables-

- And you can assign the same value to multiple variables in one line:

```py
x = y = z = "Orange"
print(x)
print(y)
print(z)
```

```py
# Orange
# Orange
# Orange
```

Unpack a Collection-

- If you have a collection of values in a list, tuple etc.
- Python allows you to extract the values into variables. This is called unpacking.

```py
fruits = ["apple", "banana", "cherry"]
x, y, z = fruits
print(x)
print(y)
print(z)
```

```py
# apple
# banana
# cherry
```

</details>

<details>
  <summary>4. Python Type Casting </summary>

If you want to specify the data type of a variable, this can be done with casting.

```py
x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0

print(x)
print(y)
print(z)
```

```py
# 3
# 3
# 3.0
```

```py
x = int(1)   # x will be 1
y = int(2.8) # y will be 2
z = int("3") # z will be 3
```

```py
x = float(1)     # x will be 1.0
y = float(2.8)   # y will be 2.8
z = float("3")   # z will be 3.0
w = float("4.2") # w will be 4.2
```

```py
x = str("s1") # x will be 's1'
y = str(2)    # y will be '2'
z = str(3.0)  # z will be '3.0'
```

</details>

<details>
  <summary>5. Python get Type </summary>

You can get the data type of a variable with the type() function.

```py
x = 5
y = "John"
print(type(x))
print(type(y))
```

```py
# <class 'int'>
# <class 'str'>
```

</details>

<details>
  <summary>6. Python Global Variables </summary>

- Variables that are created outside of a function are known as global variables.

- Global variables can be used by everyone, both inside of functions and outside.

- If you create a variable with the same name inside a function, this variable will be local, and can only be used inside the function.

- The global variable with the same name will remain as it was, global and with the original value.

- Normally, when you create a variable inside a function, that variable is local, and can only be used inside that function.

- To create a global variable inside a function, you can use the global keyword.

- Also, use the global keyword if you want to change a global variable inside a function.

```py
x = "awesome"

def myfunc():
  print("Python is " + x)

myfunc()
```

```py
# Python is awesome
```

```py
x = "awesome"

def myfunc():
  x = "fantastic"
  print("Python is " + x)

myfunc()

print("Python is " + x)
```

```py
# Python is fantastic
# Python is awesome
```

```py
def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x)
```

```py
# Python is fantastic
```

```py
x = "awesome"

def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x)
```

```py
# Python is fantastic
```

</details>

<details>
  <summary>7. Python DataTypes </summary>

- In programming, data type is an important concept.

- Variables can store data of different types, and different types can do different things.

Python has the following data types built-in by default, in these categories:

```bs
Text Type:	        str
Numeric Types:	        int, float, complex
Sequence Types:	        list, tuple, range
Mapping Type:	        dict
Set Types:	        set, frozenset
Boolean Type:	        bool
Binary Types:	        bytes, bytearray, memoryview
None Type:	        NoneType
```

str:

```bs
x = "Hello World"	str
x = str("Hello World")	str
```

int, float, complex:

```bs
x = 20	        int
x = int(20)	int

x = 20.5	float
x = float(20.5)	float

x = 1j	        complex
x = complex(1j)	complex
```

list, tuple, range:

```bs
x = ["apple", "banana", "cherry"]	    list
x = list(("apple", "banana", "cherry"))	    list

x = ("apple", "banana", "cherry")	    tuple
x = tuple(("apple", "banana", "cherry"))    tuple

x = range(6)	                            range
```

dict:

```bs
x = {"name" : "John", "age" : 36}	dict
x = dict(name="John", age=36)	        dict
```

set, frozenset:

```bs
x = {"apple", "banana", "cherry"}	set
x = set(("apple", "banana", "cherry"))	set

x = frozenset({"apple", "banana", "cherry"})	frozenset
```

bool:

```bs
x = True	bool
x = bool(5)	bool
```

bytes, bytearray, memoryview:

```bs
x = b"Hello"	            bytes
x = bytes(5)	            bytes

x = bytearray(5)	    bytearray

x = memoryview(bytes(5))    memoryview
```

NoneType:

```bs
x = None	NoneType
```

</details>

+NUMBERS

<details>
  <summary>8. Python Numbers </summary>

There are three numeric types in Python:

- int
- float
- complex

Variables of numeric types are created when you assign a value to them.

- Int, or integer, is a whole number, positive or negative, without decimals, of unlimited length.

- Float, or "floating point number" is a number, positive or negative, containing one or more decimals.

- Float can also be scientific numbers with an "e" to indicate the power of 10.

- Complex numbers are written with a "j" as the imaginary part.

- You can convert from one type to another with the int(), float(), and complex() methods.

- You cannot convert complex numbers into another number type.

```py
x = 1    # int
y = 2.8  # float
z = 1j   # complex
print(type(x))
print(type(y))
print(type(z))
```

```py
# <class 'int'>
# <class 'float'>
# <class 'complex'>
```

```py
x = 1
y = 35656222554887711
z = -3255522

print(type(x))
print(type(y))
print(type(z))
```

```py
# <class 'int'>
# <class 'int'>
# <class 'int'>
```

```py
x = 1.10
y = 1.0
z = -35.59
x = 35e3
y = 12E4
z = -87.7e100

print(type(x))
print(type(y))
print(type(z))
```

```py
# <class 'float'>
# <class 'float'>
# <class 'float'>
# <class 'float'>
# <class 'float'>
# <class 'float'>
```

```py
x = 3+5j
y = 5j
z = -5j

print(type(x))
print(type(y))
print(type(z))
```

```py
# <class 'complex'>
# <class 'complex'>
# <class 'complex'>
```

```py
x = 1    # int
y = 2.8  # float
z = 1j   # complex

#convert from int to float:
a = float(x)

#convert from float to int:
b = int(y)

#convert from int to complex:
c = complex(x)

print(a)
print(b)
print(c)

print(type(a))
print(type(b))
print(type(c))
```

```py
1.0
2
(1+0j)
<class 'float'>
<class 'int'>
<class 'complex'>
```

</details>

<details>
  <summary>9. Python Random Number </summary>

Python does not have a random() function to make a random number, but Python has a built-in module called random that can be used to make random numbers.

```py
import random

print(random.randrange(1, 10))
```

```py
# 9
```

</details>

+STRINGS

<details>
  <summary>10. Python Strings </summary>

- Strings in python are surrounded by either single quotation marks, or double quotation marks.

- 'hello' is the same as "hello".

- You can display a string literal with the print() function.

- Assigning a string to a variable is done with the variable name followed by an equal sign and the string.

- You can assign a multiline string to a variable by using three quotes.

- Square brackets can be used to access elements of the string.

```py
print("Hello")
print('Hello')
```

```py
a = "Hello"
print(a)
```

```py
a = """Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua."""
print(a)
```

```py
a = '''Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua.'''
print(a)
```

```py
# Lorem ipsum dolor sit amet,
# consectetur adipiscing elit,
# sed do eiusmod tempor incididunt
# ut labore et dolore magna aliqua.
```

```py
a = "Hello, World!"
print(a[1])
```

```py
# e
```

</details>

<details>
  <summary>11. Python Strings - Looping </summary>

- Since strings are arrays, we can loop through the characters in a string, with a for loop.

```py
for x in "banana":
  print(x)
```

```py
# b
# a
# n
# a
# n
# a
```

</details>

<details>
  <summary>12. Python Strings - Length </summary>

- To get the length of a string, use the len() function.

```py
a = "Hello, World!"
print(len(a))
```

```py
# 13
```

</details>

<details>
  <summary>13. Python Strings - Check in String </summary>

- To check if a certain phrase or character is present in a string, we can use the keyword in.

```py
txt = "The best things in life are free!"
print("free" in txt)
```

```py
# True
```

```py
txt = "The best things in life are free!"
if "free" in txt:
  print("Yes, 'free' is present.")
```

```py
# Yes, 'free' is present.
```

</details>

<details>
  <summary>14. Python Strings - Check not in String </summary>

```py
txt = "The best things in life are free!"
print("expensive" not in txt)
```

```py
# True
```

```py
txt = "The best things in life are free!"
if "expensive" not in txt:
  print("No, 'expensive' is NOT present.")
```

```py
# No, 'expensive' is NOT present.
```

</details>

<details>
  <summary>15. Python Strings - Slicing Strings </summary>

- You can return a range of characters by using the slice syntax.

- Specify the start index and the end index, separated by a colon, to return a part of the string.

- By leaving out the start index, the range will start at the first character.

- By leaving out the end index, the range will go to the end.

- Use negative indexes to start the slice from the end of the string.

```py
b = "Hello, World!"
print(b[2:5])
```

```py
# llo
```

```py
b = "Hello, World!"
print(b[:5])
```

```py
# Hello
```

```py
b = "Hello, World!"
print(b[2:])
```

```py
# llo, World!
```

```py
b = "Hello, World!"
print(b[-5:-2])
```

```py
# orl
```

</details>

<details>
  <summary>16. Python Strings - Upper and Lower Case </summary>

- The upper() method returns the string in upper case.

- The lower() method returns the string in lower case.

```py
a = "Hello, World!"
print(a.upper())
```

```py
# HELLO, WORLD!
```

```py
a = "Hello, World!"
print(a.lower())
```

```py
# hello, world!
```

</details>

<details>
  <summary>17. Python Strings - Strip (Remove) Whitespace</summary>

- Whitespace is the space before and/or after the actual text, and very often you want to remove this space.

- The strip() method removes any whitespace from the beginning or the end

```py
a = " Hello, World! "
print(a.strip()) # returns "Hello, World!"
```

```py
# Hello, World!
```

</details>

<details>
  <summary>18. Python Strings - Replace String </summary>

- The replace() method replaces a string with another string.

```py
a = "Hello, World!"
print(a.replace("H", "J"))
```

```py
# Jello, World!
```

</details>

<details>
  <summary>19. Python Strings - Split String </summary>

- The split() method returns a list where the text between the specified separator becomes the list items.

- The split() method splits the string into substrings if it finds instances of the separator.

```py
a = "Hello, World!"
print(a.split(",")) # returns ['Hello', ' World!']
```

```py
# ['Hello', ' World!']
```

</details>

<details>
  <summary>20. Python Strings - String Concatenation </summary>

- To concatenate, or combine, two strings you can use the + operator.

```py
a = "Hello"
b = "World"
c = a + b
print(c)
```

```py
# HelloWorld
```

```py
a = "Hello"
b = "World"
c = a + " " + b
print(c)
```

```py
# Hello World
```

</details>

<details>
  <summary>21. Python Strings - Format Strings </summary>

- We can combine strings and numbers by using the format() method!

- The format() method takes the passed arguments, formats them, and places them in the string where the placeholders {} are.

- The format() method takes unlimited number of arguments, and are placed into the respective placeholders.

- You can use index numbers {0} to be sure the arguments are placed in the correct placeholders.

```py
age = 36
txt = "My name is John, and I am {}"
print(txt.format(age))
```

```py
# My name is John, and I am 36
```

```py
quantity = 3
itemno = 567
price = 49.95
myorder = "I want {} pieces of item {} for {} dollars."
print(myorder.format(quantity, itemno, price))
```

```py
# I want 3 pieces of item 567 for 49.95 dollars.
```

```py
quantity = 3
itemno = 567
price = 49.95
myorder = "I want to pay {2} dollars for {0} pieces of item {1}."
print(myorder.format(quantity, itemno, price))
```

```py
# I want to pay 49.95 dollars for 3 pieces of item 567
```

</details>

<details>
  <summary>22. Python Strings - Escape Characters </summary>

- To insert characters that are illegal in a string, use an escape character.

- An escape character is a backslash \ followed by the character you want to insert.

- An example of an illegal character is a double quote inside a string that is surrounded by double quotes. To fix this problem, use the escape character \".

```py
txt = "We are the so-called \"Vikings\" from the north."
```

```py
# We are the so-called "Vikings" from the north.
```

```bs
\'	  Single Quote
\\	  Backslash
\n	  New Line
\r	  Carriage Return
\t	  Tab
\b	  Backspace
\f	  Form Feed
\ooo	  Octal value
\xhh	  Hex value
```

</details>

<details>
  <summary>23. Python Strings - capitalize() Method</summary>

- The capitalize() method returns a string where the first character is upper case, and the rest is lower case.

```bs
string.capitalize()
```

```py
txt = "hello, and welcome to my world."

x = txt.capitalize()

print (x)
```

```py
# Hello, and welcome to my world.
```

```py
txt = "python is FUN!"

x = txt.capitalize()

print (x)
```

```py
# Python is fun!
```

```py
txt = "36 is my age."

x = txt.capitalize()

print (x)
```

```py
# 36 is my age
```

</details>

<details>
  <summary>24. Python Strings - casefold() Method </summary>

- The casefold() method returns a string where all the characters are lower case.

- This method is similar to the lower() method, but the casefold() method is stronger, more aggressive, meaning that it will convert more characters into lower case, and will find more matches when comparing two strings and both are converted using the casefold() method.

```py
txt = "Hello, And Welcome To My World!"

x = txt.casefold()

print(x)
```

```py
# hello, and welcome to my world!
```

</details>

<details>
  <summary>25. Python Strings - center() Method </summary>

- The center() method will center align the string, using a specified character (space is default) as the fill character.

```bs
string.center(length, character)
```

```py
txt = "banana"

x = txt.center(20)

print(x)
```

```py
# "    banana     "
```

```py
txt = "banana"

x = txt.center(20, "O")

print(x)
```

```py
# OOOOOOObananaOOOOOOO
```

</details>

<details>
  <summary>26. Python Strings - count() Method </summary>

- The count() method returns the number of times a specified value appears in the string.

```bs
string.count(value, start, end)
```

```py
txt = "I love apples, apple are my favorite fruit"

x = txt.count("apple")

print(x)
```

```py
# 2
```

```py
txt = "I love apples, apple are my favorite fruit"

x = txt.count("apple", 10, 24)

print(x)
```

```py
# 1
```

</details>

<details>
  <summary>27. Python Strings - encode() Method </summary>

- The encode() method encodes the string, using the specified encoding. If no encoding is specified, UTF-8 will be used.

```bs
string.encode(encoding=encoding, errors=errors)
```

```py
txt = "My name is Ståle"

x = txt.encode()

print(x)
```

```py
# b'My name is St\xc3\xe5le'
```

```py
txt = "My name is Ståle"

print(txt.encode(encoding="ascii",errors="backslashreplace"))
print(txt.encode(encoding="ascii",errors="ignore"))
print(txt.encode(encoding="ascii",errors="namereplace"))
print(txt.encode(encoding="ascii",errors="replace"))
print(txt.encode(encoding="ascii",errors="xmlcharrefreplace"))
```

```py
# b'My name is St\\xe5le'
# b'My name is Stle'
# b'My name is St\\N{LATIN SMALL LETTER A WITH RING ABOVE}le'
# b'My name is St?le'
# b'My name is Ståle'
```

</details>

<details>
  <summary>28. Python Strings - endswith() Method </summary>

- The endswith() method returns True if the string ends with the specified value, otherwise False.

```bs
string.endswith(value, start, end)
```

```py
txt = "Hello, welcome to my world."

x = txt.endswith(".")

print(x)
```

```py
# True
```

```py
txt = "Hello, welcome to my world."

x = txt.endswith("my world.")

print(x)
```

```py
# True
```

```py
txt = "Hello, welcome to my world."

x = txt.endswith("my world.", 5, 11)

print(x)
```

```py
# False
```

</details>

<details>
  <summary>29. Python Strings - expandtabs() Method </summary>

- The expandtabs() method sets the tab size to the specified number of whitespaces.

```bs
string.expandtabs(tabsize)
```

```py
txt = "H\te\tl\tl\to"

x =  txt.expandtabs(2)

print(x)
```

```py
# H e l l o
```

```py
txt = "H\te\tl\tl\to"

print(txt)
print(txt.expandtabs())
print(txt.expandtabs(2))
print(txt.expandtabs(4))
print(txt.expandtabs(10))
```

```py
# H       e       l       l       o
# H       e       l       l       o
# H e l l o
# H   e   l   l   o
# H         e         l         l         o
```

</details>

<details>
  <summary>30. Python Strings - find() Method </summary>

- The find() method finds the first occurrence of the specified value.

- The find() method returns -1 if the value is not found.

- The find() method is almost the same as the index() method, the only difference is that the index() method raises an exception if the value is not found.

```bs
string.find(value, start, end)
```

```py
txt = "Hello, welcome to my world."

x = txt.find("welcome")

print(x)
```

```py
# 7
```

```py
txt = "Hello, welcome to my world."

x = txt.find("e")

print(x)
```

```py
# 1
```

```py
txt = "Hello, welcome to my world."

x = txt.find("e", 5, 10)

print(x)
```

```py
# 8
```

```py
txt = "Hello, welcome to my world."

print(txt.find("q"))
print(txt.index("q"))
```

```py
# -1
# Traceback (most recent call last):
#   File "demo_ref_string_find_vs_index.py", line 4 in <module>
#     print(txt.index("q"))
# ValueError: substring not found
```

</details>

<details>
  <summary>31. Python Strings - format() Method </summary>

- The format() method formats the specified value(s) and insert them inside the string's placeholder.

- The placeholder is defined using curly brackets: {}.

- The format() method returns the formatted string.

- The placeholders can be identified using named indexes {price}, numbered indexes {0}, or even empty placeholders {}.

```bs
string.format(value1, value2...)
```

```py
txt = "For only {price:.2f} dollars!"
print(txt.format(price = 49))
```

```py
# For only 49.00 dollars!
```

```py
txt1 = "My name is {fname}, I'm {age}".format(fname = "John", age = 36)
txt2 = "My name is {0}, I'm {1}".format("John",36)
txt3 = "My name is {}, I'm {}".format("John",36)
```

```py
# My name is John, I'm 36
# My name is John, I'm 36
# My name is John, I'm 36
```

</details>

<details>
  <summary>32. Python Strings - index() Method </summary>

- The index() method finds the first occurrence of the specified value.

- The index() method raises an exception if the value is not found.

- The index() method is almost the same as the find() method, the only difference is that the find() method returns -1 if the value is not found.

```bs
string.index(value, start, end)
```

```py
txt = "Hello, welcome to my world."

x = txt.index("welcome")

print(x)
```

```py
# 7
```

```py
txt = "Hello, welcome to my world."

x = txt.index("e")

print(x)
```

```py
# 1
```

```py
txt = "Hello, welcome to my world."

x = txt.index("e", 5, 10)

print(x)
```

```py
# 8
```

```py
txt = "Hello, welcome to my world."

print(txt.find("q"))
print(txt.index("q"))
```

```py
# -1
# Traceback (most recent call last):
#   File "demo_ref_string_find_vs_index.py", line 4 in <module>
#     print(txt.index("q"))
# ValueError: substring not found
```

</details>

<details>
  <summary>33. Python Strings - isalnum() Method </summary>

- The isalnum() method returns True if all the characters are alphanumeric, meaning alphabet letter (a-z) and numbers (0-9).

- Example of characters that are not alphanumeric: (space)!#%&? etc.

```bs
string.isalnum()
```

```py
txt = "Company12"

x = txt.isalnum()

print(x)
```

```py
# True
```

```py
txt = "Company 12"

x = txt.isalnum()

print(x)
```

```py
# False
```

</details>

<details>
  <summary>34. Python Strings - isalpha() Method </summary>

- The isalpha() method returns True if all the characters are alphabet letters (a-z).

- Example of characters that are not alphabet letters: (space)!#%&? etc.

```py
txt = "CompanyX"

x = txt.isalpha()

print(x)

```

```py
# True
```

```py
txt = "Company10"

x = txt.isalpha()

print(x)

```

```py
# False
```

</details>

<details>
  <summary>35. Python Strings - isdecimal() Method </summary>

- The isdecimal() method returns True if all the characters are decimals (0-9).

- This method is used on unicode objects.

```py
a = "\u0030" #unicode for 0
b = "\u0047" #unicode for G

print(a.isdecimal())
print(b.isdecimal())
```

```py
# True
# False
```

</details>

<details>
  <summary>36. Python Strings - isdigit() Method </summary>

- The isdigit() method returns True if all the characters are digits, otherwise False.

- Exponents, like ², are also considered to be a digit.

```py
txt = "50800"

x = txt.isdigit()

print(x)
```

```py
# True
```

```py
a = "\u0030" #unicode for 0
b = "\u00B2" #unicode for ²

print(a.isdigit())
print(b.isdigit())
```

```py
# True
# True
```

</details>

<details>
  <summary>37. Python Strings - isidentifier() Method </summary>

- The isidentifier() method returns True if the string is a valid identifier, otherwise False.

- A string is considered a valid identifier if it only contains alphanumeric letters (a-z) and (0-9), or underscores (\_).

- A valid identifier cannot start with a number, or contain any spaces.

```py
txt = "Demo"

x = txt.isidentifier()

print(x)
```

```py
# True
```

```py
a = "MyFolder"
b = "Demo002"
c = "2bring"
d = "my demo"

print(a.isidentifier())
print(b.isidentifier())
print(c.isidentifier())
print(d.isidentifier())
```

```py
# True
# True
# False
# False
```

</details>

<details>
  <summary>38. Python Strings - islower() Method </summary>

- The islower() method returns True if all the characters are in lower case, otherwise False.

- Numbers, symbols and spaces are not checked, only alphabet characters.

```py
txt = "hello world!"

x = txt.islower()

print(x)
```

```py
# True
```

```py
a = "Hello world!"
b = "hello 123"
c = "mynameisPeter"

print(a.islower())
print(b.islower())
print(c.islower())

```

```py
# False
# True
# False
```

</details>

<details>
  <summary>39. Python Strings - isnumeric() Method  </summary>

- The isnumeric() method returns True if all the characters are numeric (0-9), otherwise False.

- Exponents, like ² and ¾ are also considered to be numeric values.

- "-1" and "1.5" are NOT considered numeric values, because all the characters in the string must be numeric, and the - and the . are not.

```py
txt = "565543"

x = txt.isnumeric()

print(x)

```

```py
# True
```

```py
a = "\u0030" #unicode for 0
b = "\u00B2" #unicode for ²
c = "10km2"
d = "-1"
e = "1.5"

print(a.isnumeric())
print(b.isnumeric())
print(c.isnumeric())
print(d.isnumeric())
print(e.isnumeric())

```

```py
# True
# True
# False
# False
# False
```

</details>

<details>
  <summary>40. Python Strings - isprintable() Method </summary>

- The isprintable() method returns True if all the characters are printable, otherwise False.

- Example of none printable character can be carriage return and line feed.

```py
txt = "Hello! Are you #1?"

x = txt.isprintable()

print(x)

```

```py
# True
```

```py
txt = "Hello!\nAre you #1?"

x = txt.isprintable()

print(x)
```

```py
# False
```

</details>

<details>
  <summary>41. Python Strings - isspace() Method  </summary>

The isspace() method returns True if all the characters in a string are whitespaces, otherwise False.

```py
txt = "   "

x = txt.isspace()

print(x)
```

```py
# True
```

```py
txt = "   s   "

x = txt.isspace()

print(x)

```

```py
# False
```

</details>

<details>
  <summary>42. Python Strings - istitle() Method </summary>

- The istitle() method returns True if all words in a text start with a upper case letter, AND the rest of the word are lower case letters, otherwise False.

- Symbols and numbers are ignored.

```py
txt = "Hello, And Welcome To My World!"

x = txt.istitle()

print(x)

```

```py
# True
```

```py
a = "HELLO, AND WELCOME TO MY WORLD"
b = "Hello"
c = "22 Names"
d = "This Is %'!?"

print(a.istitle())
print(b.istitle())
print(c.istitle())
print(d.istitle())

```

```py
# False
# True
# True
# True
```

</details>

<details>
  <summary>43. Python Strings - isupper() Method  </summary>

- The isupper() method returns True if all the characters are in upper case, otherwise False.

- Numbers, symbols and spaces are not checked, only alphabet characters.

```py
txt = "THIS IS NOW!"

x = txt.isupper()

print(x)

```

```py
# True
```

```py
a = "Hello World!"
b = "hello 123"
c = "MY NAME IS PETER"

print(a.isupper())
print(b.isupper())
print(c.isupper())

```

```py
# False
# False
# True
```

</details>

<details>
  <summary>44. Python Strings - join() Method  </summary>

- The join() method takes all items in an iterable and joins them into one string.

- A string must be specified as the separator.

```py
myTuple = ("John", "Peter", "Vicky")

x = "#".join(myTuple)

print(x)
```

```py
# John#Peter#Vicky
```

```py
myDict = {"name": "John", "country": "Norway"}
mySeparator = "TEST"

x = mySeparator.join(myDict)

print(x)

```

```py
# nameTESTcountry
```

</details>

<details>
  <summary>45. Python Strings - ljust() Method </summary>

The ljust() method will left align the string, using a specified character (space is default) as the fill character.

```py
txt = "banana"

x = txt.ljust(20)

print(x, "is my favorite fruit.")
```

```py
# banana              is my favorite fruit.
```

```py
txt = "banana"

x = txt.ljust(20, "O")

print(x)

```

```py
# bananaOOOOOOOOOOOOOO
```

</details>

<details>
  <summary>46. Python Strings - lower() Method </summary>

- The lower() method returns a string where all characters are lower case.

- Symbols and Numbers are ignored.

```py
txt = "Hello my FRIENDS"

x = txt.lower()

print(x)

```

```py
# hello my friends
```

</details>

<details>
  <summary>47. Python Strings - lstrip() Method </summary>

The lstrip() method removes any leading characters (space is the default leading character to remove).

```py
txt = "     banana     "

x = txt.lstrip()

print("of all fruits", x, "is my favorite")
```

```py
# of all fruits banana     is my favorite
```

```py
txt = ",,,,,ssaaww.....banana"

x = txt.lstrip(",.asw")

print(x)

```

```py
# banana
```

</details>

<details>
  <summary>48. Python Strings - maketrans() Method </summary>

- The maketrans() method returns a mapping table that can be used with the translate() method to replace specified characters.

```py
txt = "Hello Sam!"

mytable = txt.maketrans("S", "P")

print(txt.translate(mytable))

```

```py
# Hello Pam!
```

```py
txt = "Hi Sam!"

x = "mSa"
y = "eJo"

mytable = txt.maketrans(x, y)

print(txt.translate(mytable))

```

```py
# Hi Joe!
```

```py
txt = "Good night Sam!"

x = "mSa"
y = "eJo"
z = "odnght"

mytable = txt.maketrans(x, y, z)

print(txt.translate(mytable))
```

```py
# G i Joe!
```

</details>

<details>
  <summary>49. Python Strings - partition() Method </summary>

- The partition() method searches for a specified string, and splits the string into a tuple containing three elements.

- The first element contains the part before the specified string.

- The second element contains the specified string.

- The third element contains the part after the string.

```py
txt = "I could eat bananas all day"

x = txt.partition("bananas")

print(x)

```

```py
# ('I could eat ', 'bananas', ' all day')
```

```py
txt = "I could eat bananas all day"

x = txt.partition("apples")

print(x)

```

```py
# ('I could eat bananas all day', '', '')
```

</details>

<details>
  <summary>50. Python Strings - replace() Method </summary>

The replace() method replaces a specified phrase with another specified phrase.

```py
txt = "I like bananas"

x = txt.replace("bananas", "apples")

print(x)
```

```py
# I like apples
```

```py
txt = "one one was a race horse, two two was one too."

x = txt.replace("one", "three")

print(x)

```

```py
# three three was a race horse, two two was three too."
```

```py
txt = "one one was a race horse, two two was one too."

x = txt.replace("one", "three", 2)

print(x)

```

```py
# three three was a race horse, two two was one too."
```

</details>

<details>
  <summary>51. Python Strings - rfind() Method </summary>

- The rfind() method finds the last occurrence of the specified value.

- The rfind() method returns -1 if the value is not found.

- The rfind() method is almost the same as the rindex() method.

```py
txt = "Mi casa, su casa."

x = txt.rfind("casa")

print(x)

```

```py
# 12
```

```py
txt = "Hello, welcome to my world."

x = txt.rfind("e")

print(x)

```

```py
# 13
```

```py
txt = "Hello, welcome to my world."

x = txt.rfind("e", 5, 10)

print(x)

```

```py
# 8
```

```py
txt = "Hello, welcome to my world."

print(txt.rfind("q"))
print(txt.rindex("q"))
```

```py
# -1
# Traceback (most recent call last):
#   File "demo_ref_string_rfind_vs_rindex.py", line 4 in <module>
#     print(txt.rindex("q"))
# ValueError: substring not found
```

</details>

<details>
  <summary>52. Python Strings - rindex() Method </summary>

- The rindex() method finds the last occurrence of the specified value.

- The rindex() method raises an exception if the value is not found.

- The rindex() method is almost the same as the rfind() method.

```py
txt = "Mi casa, su casa."

x = txt.rindex("casa")

print(x)

```

```py
# 12
```

```py
txt = "Hello, welcome to my world."

x = txt.rindex("e")

print(x)

```

```py
# 13
```

```py
txt = "Hello, welcome to my world."

x = txt.rindex("e", 5, 10)

print(x)
```

```py
# 8
```

```py
txt = "Hello, welcome to my world."

print(txt.rfind("q"))
print(txt.rindex("q"))
```

```py
# -1
# Traceback (most recent call last):
#   File "demo_ref_string_rfind_vs_rindex.py", line 4 in <module>
#     print(txt.rindex("q"))
# ValueError: substring not found
```

</details>

<details>
  <summary>53. Python Strings - rjust() Method  </summary>

The rjust() method will right align the string, using a specified character (space is default) as the fill character.

```py
txt = "banana"

x = txt.rjust(20)

print(x, "is my favorite fruit.")
```

```py
#                  banana is my favorite fruit.
```

```py
txt = "banana"

x = txt.rjust(20, "O")

print(x)

```

```py
# OOOOOOOOOOOOOObanana
```

</details>

<details>
  <summary>54. Python Strings - rpartition() Method </summary>

- The rpartition() method searches for the last occurrence of a specified string, and splits the string into a tuple containing three elements.

- The first element contains the part before the specified string.

- The second element contains the specified string.

- The third element contains the part after the string.

```py
txt = "I could eat bananas all day, bananas are my favorite fruit"

x = txt.rpartition("bananas")

print(x)
```

```py
# ('I could eat bananas all day, ', 'bananas', ' are my favorite fruit')
```

```py
txt = "I could eat bananas all day, bananas are my favorite fruit"

x = txt.rpartition("apples")

print(x)
```

```py
# ('', '', 'I could eat bananas all day, bananas are my favorite fruit')
```

</details>

<details>
  <summary>55. Python Strings - rsplit() Method </summary>

- The rsplit() method splits a string into a list, starting from the right.

- If no "max" is specified, this method will return the same as the split() method.

```py
txt = "apple, banana, cherry"

x = txt.rsplit(", ")

print(x)
```

```py
# ['apple', 'banana', 'cherry']
```

```py
txt = "apple, banana, cherry"

# setting the maxsplit parameter to 1, will return a list with 2 elements!
x = txt.rsplit(", ", 1)

print(x)

# note that the result has only 2 elements "apple, banana" is the first element, and "cherry" is the last.
```

```py
['apple, banana', 'cherry']
```

</details>

<details>
  <summary>56. Python Strings - rstrip() Method </summary>

The rstrip() method removes any trailing characters (characters at the end a string), space is the default trailing character to remove.

```py
txt = "     banana     "

x = txt.rstrip()

print("of all fruits", x, "is my favorite")
```

```py
# of all fruits     banana is my favorite
```

```py
txt = "banana,,,,,ssqqqww....."

x = txt.rstrip(",.qsw")

print(x)

```

```py
# banana
```

</details>

<details>
  <summary>57. Python Strings - split() Method </summary>

```py
txt = "welcome to the jungle"

x = txt.split()

print(x)
```

```py
# ['welcome', 'to', 'the', 'jungle']
```

```py
txt = "hello, my name is Peter, I am 26 years old"

x = txt.split(", ")

print(x)
```

```py
# ['hello', 'my name is Peter', 'I am 26 years old']
```

```py
txt = "apple#banana#cherry#orange"

x = txt.split("#")

print(x)

```

```py
# ['apple', 'banana', 'cherry', 'orange']
```

```py
txt = "apple#banana#cherry#orange"

# setting the maxsplit parameter to 1, will return a list with 2 elements!
x = txt.split("#", 1)

print(x)
```

```py
# ['apple', 'banana#cherry#orange']
```

</details>

<details>
  <summary>58. Python Strings - splitlines() Method </summary>

The splitlines() method splits a string into a list. The splitting is done at line breaks.

```py
txt = "Thank you for the music\nWelcome to the jungle"

x = txt.splitlines()

print(x)

```

```py
# ['Thank you for the music', 'Welcome to the jungle']
```

```py
txt = "Thank you for the music\nWelcome to the jungle"

x = txt.splitlines(True)

print(x)

```

```py
# ['Thank you for the music\n', 'Welcome to the jungle']
```

</details>

<details>
  <summary>59. Python Strings - startswith() Method </summary>

The startswith() method returns True if the string starts with the specified value, otherwise False.

```py
txt = "Hello, welcome to my world."

x = txt.startswith("Hello")

print(x)

```

```py
# True
```

```py
txt = "Hello, welcome to my world."

x = txt.startswith("wel", 7, 20)

print(x)

```

```py
# True
```

</details>

<details>
  <summary>60. Python Strings - strip() Method </summary>

The strip() method removes any leading (spaces at the beginning) and trailing (spaces at the end) characters (space is the default leading character to remove).

```py
txt = "     banana     "

x = txt.strip()

print("of all fruits", x, "is my favorite")

```

```py
# of all fruits banana is my favorite
```

```py
txt = ",,,,,rrttgg.....banana....rrr"

x = txt.strip(",.grt")

print(x)

```

```py
# banana
```

</details>

<details>
  <summary>61. Python Strings - swapcase() Method </summary>

The swapcase() method returns a string where all the upper case letters are lower case and vice versa.

```py
txt = "Hello My Name Is PETER"

x = txt.swapcase()

print(x)

```

```py
# hELLO mY nAME iS peter
```

</details>

<details>
  <summary>62. Python Strings - title() Method </summary>

- The title() method returns a string where the first character in every word is upper case. Like a header, or a title.

- If the word contains a number or a symbol, the first letter after that will be converted to upper case.

```py
txt = "Welcome to my world"

x = txt.title()

print(x)
```

```py
# Welcome To My World
```

```py
txt = "Welcome to my 2nd world"

x = txt.title()

print(x)

```

```py
# Welcome To My 2Nd World
```

</details>

<details>
  <summary>63. Python Strings - translate() Method </summary>

- The translate() method returns a string where some specified characters are replaced with the character described in a dictionary, or in a mapping table.

- Use the maketrans() method to create a mapping table.

- If a character is not specified in the dictionary/table, the character will not be replaced.

- If you use a dictionary, you must use ascii codes instead of characters.

```py
#use a dictionary with ascii codes to replace 83 (S) with 80 (P):
mydict = {83:  80}

txt = "Hello Sam!"

print(txt.translate(mydict))

```

```py
# Hello Pam!
```

```py
txt = "Hello Sam!"

mytable = txt.maketrans("S", "P")

print(txt.translate(mytable))

```

```py
# Hello Pam!
```

```py
txt = "Hi Sam!"

x = "mSa"
y = "eJo"

mytable = txt.maketrans(x, y)

print(txt.translate(mytable))

```

```py
# Hi Joe!
```

```py
txt = "Good night Sam!"

x = "mSa"
y = "eJo"
z = "odnght"

mytable = txt.maketrans(x, y, z)

print(txt.translate(mytable))

```

```py
# G i Joe!
```

```py
txt = "Good night Sam!"

mydict = {109: 101, 83: 74, 97: 111, 111: None, 100: None, 110: None, 103: None, 104: None, 116: None}

print(txt.translate(mydict))

```

```py
# G i Joe!
```

</details>

<details>
  <summary>64. Python Strings - upper() Method </summary>

- The upper() method returns a string where all characters are in upper case.

- Symbols and Numbers are ignored.

```py
txt = "Hello my friends"

x = txt.upper()

print(x)

```

```py
# HELLO MY FRIENDS
```

</details>

<details>
  <summary>65. Python Strings - zfill() Method </summary>

- The zfill() method adds zeros (0) at the beginning of the string, until it reaches the specified length.

- If the value of the len parameter is less than the length of the string, no filling is done.

```py
txt = "50"

x = txt.zfill(10)

print(x)

```

```py
# 0000000050
```

```py
a = "hello"
b = "welcome to the jungle"
c = "10.000"

print(a.zfill(10))
print(b.zfill(10))
print(c.zfill(10))
```

```py
# 00000hello
# welcome to the jungle
# 000010.000
```

</details>

<details>
  <summary>66. Python isinstance() </summary>

Python also has many built-in functions that return a boolean value, like the isinstance() function, which can be used to determine if an object is of a certain data type

```py
x = 200
print(isinstance(x, int))
```

```py
# True
```

</details>

+LISTS

<details>
  <summary>67. Python Lists - Introduction </summary>

- Lists are used to store multiple items in a single variable.

- Lists are one of 4 built-in data types in Python used to store collections of data, the other 3 are Tuple, Set, and Dictionary, all with different qualities and usage.

- Lists are created using square brackets.

- List items are ordered, changeable, and allow duplicate values.

- List items are indexed, the first item has index [0], the second item has index [1] etc.

- The list is changeable, meaning that we can change, add, and remove items in a list after it has been created.

There are four collection data types in the Python programming language:

- List is a collection which is ordered and changeable. Allows duplicate members.
- Tuple is a collection which is ordered and unchangeable. Allows duplicate members.
- Set is a collection which is unordered, unchangeable\*, and unindexed. No duplicate members.
- Dictionary is a collection which is ordered\*\* and changeable. No duplicate members.

```py
thislist = ["apple", "banana", "cherry"]
print(thislist)
```

```py
# ['apple', 'banana', 'cherry']
```

</details>

<details>
  <summary>68. Python Lists - Length</summary>

To determine how many items a list has, use the len() function.

```py
thislist = ["apple", "banana", "cherry"]
print(len(thislist))
```

```py
# 3
```

</details>

<details>
  <summary>69. Python Lists - Data type </summary>

```py
mylist = ["apple", "banana", "cherry"]

print(type(mylist))

```

```py
# <class 'list'>
```

</details>

<details>
  <summary>70. Python Lists - list() Constructor </summary>

```py
thislist = list(("apple", "banana", "cherry"))
print(thislist)

```

```py
# ['apple', 'banana', 'cherry']
```

</details>

<details>
  <summary>71. Python Lists - Access Items</summary>

```py
thislist = ["apple", "banana", "cherry"]
print(thislist[1])

```

```py
# banana
```

```py
thislist = ["apple", "banana", "cherry"]
print(thislist[-1])

```

```py
# cherry
```

```py
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[2:5])

#This will return the items from position 2 to 5.

#Remember that the first item is position 0,
#and note that the item in position 5 is NOT included

```

```py
# ['cherry', 'orange', 'kiwi']
```

```py
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[:4])

#This will return the items from index 0 to index 4.

#Remember that index 0 is the first item, and index 4 is the fifth item
#Remember that the item in index 4 is NOT included

```

```py
# ['apple', 'banana', 'cherry', 'orange']
```

```py
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[2:])

#This will return the items from index 2 to the end.

#Remember that index 0 is the first item, and index 2 is the third
```

```py
# ['cherry', 'orange', 'kiwi', 'melon', 'mango']
```

```py
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[-4:-1])

#Negative indexing means starting from the end of the list.

#This example returns the items from index -4 (included) to index -1 (excluded)

#Remember that the last item has the index -1,

```

```py
# ['orange', 'kiwi', 'melon']
```

</details>

<details>
  <summary>72. Python Lists - Check if Item Exists </summary>

```py
thislist = ["apple", "banana", "cherry"]
if "apple" in thislist:
  print("Yes, 'apple' is in the fruits list")
```

```py
# Yes, 'apple' is in the fruits list
```

</details>

<details>
  <summary>73. Python Lists - Change Item Value</summary>

```py
thislist = ["apple", "banana", "cherry"]
thislist[1] = "blackcurrant"

print(thislist)

```

```py
# ['apple', 'blackcurrant', 'cherry']
```

```py
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "mango"]

thislist[1:3] = ["blackcurrant", "watermelon"]

print(thislist)

```

```py
# ['apple', 'blackcurrant', 'watermelon', 'orange', 'kiwi', 'mango']
```

```py
thislist = ["apple", "banana", "cherry"]

thislist[1:2] = ["blackcurrant", "watermelon"]

print(thislist)

```

```py
# ['apple', 'blackcurrant', 'watermelon', 'cherry']
```

```py
thislist = ["apple", "banana", "cherry"]

thislist[1:3] = ["watermelon"]

print(thislist)

```

```py
# ['apple', 'watermelon']
```

</details>

<details>
  <summary>74. Python Lists - Insert() method </summary>

- To insert a new list item, without replacing any of the existing values, we can use the insert() method.

- The insert() method inserts an item at the specified index.

```py
thislist = ["apple", "banana", "cherry"]

thislist.insert(2, "watermelon")

print(thislist)

```

```py
# ['apple', 'banana', 'watermelon', 'cherry']
```

```py
thislist = ["apple", "banana", "cherry"]
thislist.insert(1, "orange")
print(thislist)

```

```py
# ['apple', 'orange', 'banana', 'cherry']
```

</details>

<details>
  <summary>75. Python Lists - Append() method </summary>

To add an item to the end of the list, use the append() method.

```py
thislist = ["apple", "banana", "cherry"]

thislist.append("orange")

print(thislist)

```

```py
# ['apple', 'banana', 'cherry', 'orange']
```

</details>

<details>
  <summary>76. Python Lists - Extend() method</summary>

To append elements from another list to the current list, use the extend() method.

```py
thislist = ["apple", "banana", "cherry"]
tropical = ["mango", "pineapple", "papaya"]

thislist.extend(tropical)

print(thislist)

```

```py
# ['apple', 'banana', 'cherry', 'mango', 'pineapple', 'papaya']
```

```py
thislist = ["apple", "banana", "cherry"]
thistuple = ("kiwi", "orange")

thislist.extend(thistuple)

print(thislist)

```

```py
# ['apple', 'banana', 'cherry', 'kiwi', 'orange']
```

</details>

<details>
  <summary>77. Python Lists - remove() method </summary>

The remove() method removes the specified item.

```py
thislist = ["apple", "banana", "cherry"]
thislist.remove("banana")
print(thislist)

```

```py
# ['apple', 'cherry']
```

</details>

<details>
  <summary>78. Python Lists - pop() method </summary>

The pop() method removes the specified index.

```py
thislist = ["apple", "banana", "cherry"]
thislist.pop(1)
print(thislist)

```

```py
# ['apple', 'cherry']
```

```py
thislist = ["apple", "banana", "cherry"]
thislist.pop()
print(thislist)

```

```py
# ['apple', 'banana']
```

</details>

<details>
  <summary>79. Python Lists - del keyword </summary>

The del keyword also removes the specified index.

```py
thislist = ["apple", "banana", "cherry"]
del thislist[0]
print(thislist)

```

```py
# ['banana', 'cherry']
```

```py
thislist = ["apple", "banana", "cherry"]
del thislist
print(thislist) #this will cause an error because you have succsesfully deleted "thislist".
```

```py
# Traceback (most recent call last):
#   File "demo_list_del2.py", line 3, in <module>
#     print(thislist) #this will cause an error because you have succsesfully deleted "thislist".
# NameError: name 'thislist' is not defined
```

</details>

<details>
  <summary>80. Python Lists - clear() method </summary>

- The clear() method empties the list.

- The list still remains, but it has no content.

```py
thislist = ["apple", "banana", "cherry"]
thislist.clear()
print(thislist)
```

```py
# []
```

</details>

<details>
  <summary>81. Python Lists - Loop Through a List </summary>

You can loop through the list items by using a for loop.

```py
thislist = ["apple", "banana", "cherry"]
for x in thislist:
  print(x)

```

```py
# apple
# banana
# cherry
```

</details>

<details>
  <summary>82. Python Lists - Loop Through the Index Numbers</summary>

- You can also loop through the list items by referring to their index number.

- Use the range() and len() functions to create a suitable iterable.

```py
thislist = ["apple", "banana", "cherry"]
for i in range(len(thislist)):
  print(thislist[i])
```

```py
# apple
# banana
# cherry
```

</details>

<details>
  <summary>83. Python Lists - While Loop </summary>

- You can loop through the list items by using a while loop.

- Use the len() function to determine the length of the list, then start at 0 and loop your way through the list items by referring to their indexes.

- Remember to increase the index by 1 after each iteration.

```py
thislist = ["apple", "banana", "cherry"]
i = 0
while i < len(thislist):
  print(thislist[i])
  i = i + 1

```

```py
# apple
# banana
# cherry
```

</details>

<details>
  <summary>84. Python Lists - List Comprehension</summary>

The Syntax:

```bs
newlist = [expression for item in iterable if condition == True]
```

List Comprehension offers the shortest syntax for looping through lists.

```py
thislist = ["apple", "banana", "cherry"]
[print(x) for x in thislist]

```

```py
# apple
# banana
# cherry
```

```py
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]
newlist = []

for x in fruits:
  if "a" in x:
    newlist.append(x)

print(newlist)

```

```py
# ['apple', 'banana', 'mango']
```

```py
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]
newlist = [x for x in fruits if "a" in x]

print(newlist)

```

```py
# ['apple', 'banana', 'mango']
```

```py
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]

newlist = [x for x in fruits if x != "apple"]

print(newlist)

```

```py
# ['banana', 'cherry', 'kiwi', 'mango']
```

```py
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]

newlist = [x for x in fruits]

print(newlist)

```

```py
# ['apple', 'banana', 'cherry', 'kiwi', 'mango']
```

```py
newlist = [x for x in range(10)]

print(newlist)

```

```py
# [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```

```py
newlist = [x for x in range(10) if x < 5]

print(newlist)

```

```py
# [0, 1, 2, 3, 4]
```

```py
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]

newlist = [x.upper() for x in fruits]

print(newlist)

```

```py
# ['APPLE', 'BANANA', 'CHERRY', 'KIWI', 'MANGO']
```

```py
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]

newlist = ['hello' for x in fruits]

print(newlist)

```

```py
# ['hello', 'hello', 'hello', 'hello', 'hello']
```

```py
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]

newlist = [x if x != "banana" else "orange" for x in fruits]

print(newlist)

```

```py
# ['apple', 'orange', 'cherry', 'kiwi', 'mango']
```

</details>

<details>
  <summary>85. Python Lists - Sort Ascending </summary>

List objects have a sort() method that will sort the list alphanumerically, ascending, by default.

```py
thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]

thislist.sort()

print(thislist)

```

```py
# ['banana', 'kiwi', 'mango', 'orange', 'pineapple']
```

```py
thislist = [100, 50, 65, 82, 23]

thislist.sort()

print(thislist)

```

```py
# [23, 50, 65, 82, 100]
```

</details>

<details>
  <summary>86. Python Lists - Sort Descending</summary>

```py
thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]

thislist.sort(reverse = True)

print(thislist)

```

```py
# ['pineapple', 'orange', 'mango', 'kiwi', 'banana']
```

```py
thislist = [100, 50, 65, 82, 23]

thislist.sort(reverse = True)

print(thislist)

```

```py
# [100, 82, 65, 50, 23]
```

</details>

<details>
  <summary>87. Python Lists - Customize Sort </summary>

```py
def myfunc(n):
  return abs(n - 50)

thislist = [100, 50, 65, 82, 23]

thislist.sort(key = myfunc)

print(thislist)

```

```py
# [50, 65, 23, 82, 100]
```

</details>

<details>
  <summary>88. Python Lists - Case Insensitive </summary>

By default the sort() method is case sensitive, resulting in all capital letters being sorted before lower case letters.

```py
thislist = ["banana", "Orange", "Kiwi", "cherry"]

thislist.sort()

print(thislist)

```

```py
# ['Kiwi', 'Orange', 'banana', 'cherry']
```

```py
thislist = ["banana", "Orange", "Kiwi", "cherry"]

thislist.sort(key = str.lower)

print(thislist)

```

```py
# ['banana', 'cherry', 'Kiwi', 'Orange']
```

</details>

<details>
  <summary>89. Python Lists - Reverse Order of List </summary>

- What if you want to reverse the order of a list, regardless of the alphabet?

- The reverse() method reverses the current sorting order of the elements.

```py
thislist = ["banana", "Orange", "Kiwi", "cherry"]

thislist.reverse()

print(thislist)

```

```py
# ['cherry', 'Kiwi', 'Orange', 'banana']
```

</details>

<details>
  <summary>99. Python Lists - Copy Lists </summary>

- You cannot copy a list simply by typing list2 = list1, because: list2 will only be a reference to list1, and changes made in list1 will automatically also be made in list2.

- There are ways to make a copy, one way is to use the built-in List method copy().

- Another way to make a copy is to use the built-in method list().

```py
thislist = ["apple", "banana", "cherry"]
mylist = thislist.copy()
print(mylist)

```

```py
# ['apple', 'banana', 'cherry']
```

```py
thislist = ["apple", "banana", "cherry"]
mylist = list(thislist)
print(mylist)

```

```py
# ['apple', 'banana', 'cherry']
```

</details>

<details>
  <summary>100. Python Lists - Join Lists</summary>

- There are several ways to join, or concatenate, two or more lists in Python.

- One of the easiest ways are by using the + operator.

- Another way to join two lists is by appending all the items from list2 into list1, one by one.

- Or you can use the extend() method, which purpose is to add elements from one list to another list.

```py
list1 = ["a", "b", "c"]
list2 = [1, 2, 3]

list3 = list1 + list2
print(list3)

```

```py
# ['a', 'b', 'c', 1, 2, 3]
```

```py
list1 = ["a", "b" , "c"]
list2 = [1, 2, 3]

for x in list2:
  list1.append(x)

print(list1)

```

```py
# ['a', 'b', 'c', 1, 2, 3]
```

```py
list1 = ["a", "b" , "c"]
list2 = [1, 2, 3]

list1.extend(list2)
print(list1)

```

```py
# ['a', 'b', 'c', 1, 2, 3]
```

</details>

<details>
  <summary>101. Python Lists - count() Method </summary>

The count() method returns the number of elements with the specified value.

```py
fruits = ["apple", "banana", "cherry"]

x = fruits.count("cherry")

print(x)

```

```py
# 1
```

```py
fruits = [1, 4, 2, 9, 7, 8, 9, 3, 1]

x = fruits.count(9)

print(x)

```

```py
# 2
```

</details>

<details>
  <summary>102. Python Lists - extend() Method </summary>

The extend() method adds the specified list elements (or any iterable) to the end of the current list.

```py
fruits = ['apple', 'banana', 'cherry']

cars = ['Ford', 'BMW', 'Volvo']

fruits.extend(cars)

print(fruits)
```

```py
# ['apple', 'banana', 'cherry', 'Ford', 'BMW', 'Volvo']
```

```py
fruits = ['apple', 'banana', 'cherry']

points = (1, 4, 5, 9)

fruits.extend(points)

print(fruits)

```

```py
# ['apple', 'banana', 'cherry', 1, 4, 5, 9]
```

</details>

<details>
  <summary>103. Python Lists - index() Method </summary>

The index() method returns the position at the first occurrence of the specified value.

```py
fruits = ['apple', 'banana', 'cherry']

x = fruits.index("cherry")

print(x)

```

```py
# 2
```

```py
fruits = [4, 55, 64, 32, 16, 32]

x = fruits.index(32)

print(x)

```

```py
# 3
```

</details>

<details>
  <summary>104. Python Lists - reverse() Method </summary>

The reverse() method reverses the sorting order of the elements.

```py
fruits = ['apple', 'banana', 'cherry']

fruits.reverse()

print(fruits)

```

```py
# ['cherry', 'banana', 'apple']
```

</details>

<details>
  <summary>105. Python Lists - sort() Method </summary>

- The sort() method sorts the list ascending by default.

- You can also make a function to decide the sorting criteria(s).

```py
cars = ['Ford', 'BMW', 'Volvo']

cars.sort()

print(cars)

```

```py
# ['BMW', 'Ford', 'Volvo']
```

```py
cars = ['Ford', 'BMW', 'Volvo']

cars.sort(reverse=True)

print(cars)

```

```py
# ['Volvo', 'Ford', 'BMW']
```

```py
# A function that returns the length of the value:
def myFunc(e):
  return len(e)

cars = ['Ford', 'Mitsubishi', 'BMW', 'VW']

cars.sort(key=myFunc)

print(cars)

```

```py
# ['VW', 'BMW', 'Ford', 'Mitsubishi']
```

```py
def myFunc(e):
  return e['year']

cars = [
  {'car': 'Ford', 'year': 2005},
  {'car': 'Mitsubishi', 'year': 2000},
  {'car': 'BMW', 'year': 2019},
  {'car': 'VW', 'year': 2011}
]

cars.sort(key=myFunc)

print(cars)

```

```py
# [{'car': 'Mitsubishi', 'year': 2000}, {'car': 'Ford', 'year': 2005}, {'car': 'VW', 'year': 2011}, {'car': 'BMW', 'year': 2019}]
```

```py
# A function that returns the length of the value:
def myFunc(e):
  return len(e)

cars = ['Ford', 'Mitsubishi', 'BMW', 'VW']

cars.sort(reverse=True, key=myFunc)

print(cars)

```

```py
# ['Mitsubishi', 'Ford'', 'BMW', 'VW']
```

</details>

+TUPLES

<details>
  <summary>106. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>107. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>108. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>109. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>110. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>111. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>112. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>113. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>114. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>115. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>116. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>117. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>118. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>119. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>120. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>121. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>122. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>123. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>124. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>125. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>126. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>127. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>128. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>129. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>130. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>131. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>132. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>133. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>134. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>135. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>136. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>137. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>138. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>139. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>140. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>141. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>142. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>143. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>144. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>145. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>146. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>147. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>148. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>149. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>150. Python Tuples - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

### [2-DJANGO TUTORIAL - W3SCHOOLS](#)

+INTRODUCTION

<details>
  <summary>A1. Introduction </summary>

Django follows the MVT design pattern (Model View Template).

- Model - The data you want to present, usually data from a database.
- View - A request handler that returns the relevant template and content - based on the request from the user.
- Template - A text file (like an HTML file) containing the layout of the web page, with logic on how to display the data.

Model <br>

The model provides data from the database.

- In Django, the data is delivered as an Object Relational Mapping (ORM), which is a technique designed to make it easier to work with databases.

- The most common way to extract data from a database is SQL. One problem with SQL is that you have to have a pretty good understanding of the database structure to be able to work with it.

- Django, with ORM, makes it easier to communicate with the database, without having to write complex SQL statements.

- The models are usually located in a file called models.py.

View

- A view is a function or method that takes http requests as arguments, imports the relevant model(s), and finds out what data to send to the template, and returns the final result.

- The views are usually located in a file called views.py.

Template

- A template is a file where you describe how the result should be represented.

- Templates are often .html files, with HTML code describing the layout of a web page, but it can also be in other file formats to present other results, but we will concentrate on .html files.

- Django uses standard HTML to describe the layout, but uses Django tags to add logic.

- The templates of an application is located in a folder named templates.

```html
<h1>My Homepage</h1>

<p>My name is {{ firstname }}.</p>
```

URLs

- Django also provides a way to navigate around the different pages in a website.

- When a user requests a URL, Django decides which view it will send it to.

- This is done in a file called urls.py.

</details>

<details>
  <summary>A2. Install Python, pip and Venv </summary>

Download Python:

```py
https://www.python.org/
```

Check for Python Version:

```py
python --version
```

```py
# Python 3.9.12
```

Install pip:

```py
https://pypi.org/project/pip/
```

Check pip version:

```py
pip --version
```

```py
# pip 21.2.4
```

Upgrade pip:

```py
python -m pip install --upgrade pip
```

Install venv and activate the virtual environment:

```py
python -m venv venv-w3django

source venv-w3django/bin/activate
```

</details>

<details>
  <summary>A3. Install Django </summary>

```py
python -m pip install Django
```

Check Django version:

```py
django-admin --version
```

```py
# 4.1.5
```

</details>

<details>
  <summary>A4. Create Django Project </summary>

```py
django-admin startproject my_tennis_club
django-admin startproject my_tennis_club .
```

run django project -

my_tennis_club/

```py
python manage.py runserver
```

```py
# System check identified no issues (0 silenced).

# You have 18 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s): admin, auth, contenttypes, sessions.
# Run 'python manage.py migrate' to apply them.
# January 26, 2023 - 19:26:37
# Django version 4.1.5, using settings 'my_tennis_club.settings'
# Starting development server at http://127.0.0.1:8000/
# Quit the server with CONTROL-C.
```

127.0.0.1:8000:

![001](https://user-images.githubusercontent.com/32337103/214931443-5581766b-920d-4ddb-ac99-c649421fa3d1.png)

</details>

<details>
  <summary>A5. Create Django App </summary>

my_tennis_club/

```py
python manage.py startapp members
```

</details>

<details>
  <summary>A6. Create Django View - return HttpResponse </summary>

members/views.py:

```py
from django.shortcuts import render
from django.http import HttpResponse

def members(request):
    return HttpResponse("Hello world!")
```

</details>

<details>
  <summary>A7. Create urls.py routes </summary>

my_tennis_club/members/urls.py:

```py
from django.urls import path
from . import views

urlpatterns = [
    path('members/', views.members, name='members'),
]
```

my_tennis_club/my_tennis_club/urls.py:

```py
from django.contrib import admin
from django.urls import include, path

urlpatterns = [
    path('', include('members.urls')),
    path('admin/', admin.site.urls),
]
```

/my_tennis_club:

```py
python manage.py runserver
```

127.0.0.1:8000/members:

![002](https://user-images.githubusercontent.com/32337103/214957810-f91a2461-1028-4d23-bcd4-9ef782e741e4.png)

</details>

<details>
  <summary>A8. Create and load HTML Template </summary>

my_tennis_club/members/templates/myfirst.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>Hello World!</h1>
    <p>Welcome to my first Django project!</p>
  </body>
</html>
```

my_tennis_club/members/views.py:

```py
from django.http import HttpResponse
from django.template import loader

def members(request):
  template = loader.get_template('myfirst.html')
  return HttpResponse(template.render())
```

</details>

<details>
  <summary>A9. Register App in Settings </summary>

my_tennis_club/my_tennis_club/settings.py:

```py
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'members'
]
```

Run Migrations:

```py
# python manage.py makemigrations
python manage.py migrate
```

/my_tennis_club

```py
python manage.py runserver
```

127.0.0.1:8000/members:

![004](https://user-images.githubusercontent.com/32337103/214960898-da8f5076-7b10-4112-a4cd-f9d12589fc5d.png)

</details>

<details>
  <summary>A10. Create Member Model </summary>

my_tennis_club/members/models.py:

```py
from django.db import models

class Member(models.Model):
  firstname = models.CharField(max_length=255)
  lastname = models.CharField(max_length=255)
```

my_tennis_club/

```py
python manage.py makemigrations members
```

```py
python manage.py migrate
```

View SQL migrate:

```py
python manage.py sqlmigrate <model> <migration number>
python manage.py sqlmigrate members 0001
```

```py
# BEGIN;
# --
# -- Create model Member
# --
# CREATE TABLE "members_member" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "firstname" varchar(255) NOT NULL, "lastname" varchar(255) NOT NULL);
# COMMIT;
```

</details>

<details>
  <summary>A11. Get and Insert Data </summary>

Enter Python Shell

```py
python manage.py shell
```

```py
# Python 3.9.13 (v3.9.13:6de2ca5339, May 17 2022, 11:37:23)
# [Clang 13.0.0 (clang-1300.0.29.30)] on darwin
# Type "help", "copyright", "credits" or "license" for more information.
# (InteractiveConsole)
# >>>
```

GET Data from Members Table (Model):

```py
>>> from members.models import Member
>>> Member.objects.all()
```

```py
# <QuerySet []>
```

POST/Add a single Data record to Members Table (Model):

```py
>>> member = Member(firstname='Emil', lastname='Refsnes')
>>> member.save()
```

View added record in Model:

```py
>>> Member.objects.all()
```

```py
# <QuerySet [<Member: Member object (1)>]>
```

```py
>>> Member.objects.all().values()
```

```py
# <QuerySet [{'id': 1, 'firstname': 'Emil', 'lastname': 'Refsnes'}]>
```

To add Multiple Records in the Model:

```py
>>> member1 = Member(firstname='Tobias', lastname='Refsnes')
>>> member2 = Member(firstname='Linus', lastname='Refsnes')
>>> member3 = Member(firstname='Lene', lastname='Refsnes')
>>> member4 = Member(firstname='Stale', lastname='Refsnes')
>>> member5 = Member(firstname='Jane', lastname='Doe')
>>> members_list = [member1, member2, member3, member4, member5]
>>> for x in members_list:
>>>   x.save()
```

View added records in Model:

```py
>>> Member.objects.all().values()
```

```py
# <QuerySet [{'id': 1, 'firstname': 'Emil', 'lastname': 'Refsnes'},
# {'id': 2, 'firstname': 'Tobias', 'lastname': 'Refsnes'},
# {'id': 3, 'firstname': 'Linus', 'lastname': 'Refsnes'},
# {'id': 4, 'firstname': 'Lene', 'lastname': 'Refsnes'},
# {'id': 5, 'firstname': 'Stale', 'lastname': 'Refsnes'},
# {'id': 6, 'firstname': 'Jane', 'lastname': 'Doe'}]>
```

</details>

<details>
  <summary>12. Update Data Records </summary>

Get the record for member at index 4, which is "Stale Refsnes":

```py
>>> from members.models import Member
>>> x = Member.objects.all()[4]
>>> x.firstname
```

```py
# 'Stale'
```

Now change the value of this record:

```py
>>> x.firstname = "Stalikken"
>>> x.save()
```

```py
>>> Member.objects.all().values()
```

```py
# <QuerySet [{'id': 1, 'firstname': 'Emil', 'lastname': 'Refsnes'},
# {'id': 2, 'firstname': 'Tobias', 'lastname': 'Refsnes'},
# {'id': 3, 'firstname': 'Linus', 'lastname': 'Refsnes'},
# {'id': 4, 'firstname': 'Lene', 'lastname': 'Refsnes'},
# {'id': 5, 'firstname': 'Stalikken', 'lastname': 'Refsnes'},
# {'id': 6, 'firstname': 'Jane', 'lastname': 'Doe'}]>
```

</details>

<details>
  <summary>13. Delete Data Records </summary>

Get the record you want to delete:

```py
>>> from members.models import Member
>>> x = Member.objects.all()[5]
>>> x.firstname
```

```py
# 'Jane'
```

Now delete the record:

```py
>>> x.delete()
```

```py
# (1, {'members.Member': 1})
```

```py
>>> Member.objects.all().values()
```

```py
# <QuerySet [{'id': 1, 'firstname': 'Emil', 'lastname': 'Refsnes'},
# {'id': 2, 'firstname': 'Tobias', 'lastname': 'Refsnes'},
# {'id': 3, 'firstname': 'Linus', 'lastname': 'Refsnes'},
# {'id': 4, 'firstname': 'Lene', 'lastname': 'Refsnes'},
# {'id': 5, 'firstname': 'Stalikken', 'lastname': 'Refsnes'}]>
```

```py
>>> exit()
```

</details>

<details>
  <summary>14. Add Fields (Columns) to Model </summary>

my_tennis_club/members/models.py:

```py
from django.db import models

class Member(models.Model):
  firstname = models.CharField(max_length=255)
  lastname = models.CharField(max_length=255)
  phone = models.IntegerField()
  joined_date = models.DateField()
```

Make Migrations:

```py
python manage.py makemigrations members
```

```py
# You are trying to add a non-nullable field 'joined_date' to members without a default; we can't do that (the database needs something to populate existing rows).
# Please select a fix:
#  1) Provide a one-off default now (will be set on all existing rows with a null value for this column)
#  2) Quit, and let me add a default in models.py
# Select an option:
```

```bs
Select option 2: allow NULL values for the two new fields.
```

my_tennis_club/members/models.py:

```py
from django.db import models

class Member(models.Model):
  firstname = models.CharField(max_length=255)
  lastname = models.CharField(max_length=255)
  phone = models.IntegerField(null=True)
  joined_date = models.DateField(null=True)
```

Make Migrations:

```py
python manage.py makemigrations members
```

```py
# Migrations for 'members':
#   members/migrations/0002_member_joined_date_member_phone.py
#     - Add field joined_date to member
#     - Add field phone to member
```

Run the migrate command:

```py
python manage.py migrate
```

```py
# Operations to perform:
#   Apply all migrations: admin, auth, contenttypes, members, sessions
# Running migrations:
#   Applying members.0002_member_joined_date_member_phone... OK
```

</details>

<details>
  <summary>15. Insert Data into updated Model </summary>

```py
python manage.py shell
```

```py
# Python 3.9.2 (tags/v3.9.2:1a79785, Feb 19 2021, 13:44:55) [MSC v.1928 64 bit (AMD64)] on win32
# Type "help", "copyright", "credits" or "license" for more information.
# (InteractiveConsole)
# >>>
```

```py
>>> from members.models import Member
>>> x = Member.objects.all()[0]
>>> x.phone = 5551234
>>> x.joined_date = '2022-01-05'
>>> x.save()
```

```py
>>> Member.objects.all().values()
```

```py
# <QuerySet [
# {'id': 1, 'firstname': 'Emil', 'lastname': 'Refsnes', 'phone': 5551234, 'joined_date': datetime.date(2022, 1, 5)},
# {'id': 2, 'firstname': 'Tobias', 'lastname': 'Refsnes', 'phone': None, 'joined_date': None},
# {'id': 3, 'firstname': 'Linus', 'lastname': 'Refsnes', 'phone': None, 'joined_date': None},
# {'id': 4, 'firstname': 'Lene', 'lastname': 'Refsnes', 'phone': None, 'joined_date': None},
# {'id': 5, 'firstname': 'Stalikken', 'lastname': 'Refsnes', 'phone': None, 'joined_date': None}]>
```

</details>

+DISPLAY TEMPLATE DATA

<details>
  <summary>16. Create All Members Page </summary>

my_tennis_club/members/templates/all_members.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>Members</h1>

    <ul>
      {% for x in mymembers %}
      <li>{{ x.firstname }} {{ x.lastname }}</li>
      {% endfor %}
    </ul>
  </body>
</html>
```

my_tennis_club/members/views.py:

```py
from django.http import HttpResponse
from django.template import loader
from .models import Member

def members(request):
  mymembers = Member.objects.all().values()
  template = loader.get_template('all_members.html')
  context = {
    'mymembers': mymembers,
  }
  return HttpResponse(template.render(context, request))
```

my_tennis_club/members/urls.py:

```py
from django.urls import path
from . import views

urlpatterns = [
    path('members/', views.members, name='members'),
]
```

my_tennis_club/

```py
python manage.py runserver
```

![004](https://user-images.githubusercontent.com/32337103/215118713-ad8cf2c0-cb2a-497d-b558-bc273b8245bc.png)

</details>

<details>
  <summary>17. Create Details Page </summary>

my_tennis_club/members/templates/details.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>{{ mymember.firstname }} {{ mymember.lastname }}</h1>

    <p>Phone: {{ mymember.phone }}</p>
    <p>Member since: {{ mymember.joined_date }}</p>

    <p>Back to <a href="/members">Members</a></p>
  </body>
</html>
```

my_tennis_club/members/templates/all_members.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>Members</h1>

    <ul>
      {% for x in mymembers %}
      <li>
        <a href="details/{{ x.id }}">{{ x.firstname }} {{ x.lastname }}</a>
      </li>
      {% endfor %}
    </ul>
  </body>
</html>
```

my_tennis_club/members/views.py:

```py
from django.http import HttpResponse
from django.template import loader
from .models import Member

def members(request):
  mymembers = Member.objects.all().values()
  template = loader.get_template('all_members.html')
  context = {
    'mymembers': mymembers,
  }
  return HttpResponse(template.render(context, request))

def details(request, id):
  mymember = Member.objects.get(id=id)
  template = loader.get_template('details.html')
  context = {
    'mymember': mymember,
  }
  return HttpResponse(template.render(context, request))
```

my_tennis_club/members/urls.py:

```py
from django.urls import path
from . import views

urlpatterns = [
    path('members/', views.members, name='members'),
    path('members/details/<int:id>', views.details, name='details'),
]
```

```py
py manage.py runserver
```

![006](https://user-images.githubusercontent.com/32337103/215122475-c5df9fb6-5c0e-4e6e-8dff-3a7078130f4c.png)

![007](https://user-images.githubusercontent.com/32337103/215122533-7600e321-0f0a-4a66-b7df-ea43fcdc6de1.png)

</details>

<details>
  <summary>18. Create Master Layout Page </summary>

my_tennis_club/members/templates/master.html:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>{% block title %}{% endblock %}</title>
  </head>
  <body>
    {% block content %} {% endblock %}
  </body>
</html>
```

my_tennis_club/members/templates/all_members.html:

```bs
{% extends "master.html" %}

{% block title %}
  My Tennis Club - List of all members
{% endblock %}


{% block content %}
  <h1>Members</h1>

  <ul>
    {% for x in mymembers %}
      <li><a href="details/{{ x.id }}">{{ x.firstname }} {{ x.lastname }}</a></li>
    {% endfor %}
  </ul>
{% endblock %}
```

my_tennis_club/members/templates/details.html:

```bs
{% extends "master.html" %}

{% block title %}
  Details about {{ mymember.firstname }} {{ mymember.lastname }}
{% endblock %}


{% block content %}
  <h1>{{ mymember.firstname }} {{ mymember.lastname }}</h1>

  <p>Phone {{ mymember.phone }}</p>
  <p>Member since: {{ mymember.joined_date }}</p>

  <p>Back to <a href="/members">Members</a></p>

{% endblock %}
```

```py
py manage.py runserver
```

![006](https://user-images.githubusercontent.com/32337103/215122475-c5df9fb6-5c0e-4e6e-8dff-3a7078130f4c.png)

![007](https://user-images.githubusercontent.com/32337103/215122533-7600e321-0f0a-4a66-b7df-ea43fcdc6de1.png)

</details>

<details>
  <summary>19. Create Main Landing Page </summary>

my_tennis_club/members/templates/main.html:

```bash
{% extends "master.html" %}

{% block title %}
  My Tennis Club
{% endblock %}


{% block content %}
  <h1>My Tennis Club</h1>

  <h3>Members</h3>

  <p>Check out all our <a href="members/">members</a></p>

{% endblock %}
```

my_tennis_club/members/views.py:

```py
from django.http import HttpResponse
from django.template import loader
from .models import Member

def members(request):
  mymembers = Member.objects.all().values()
  template = loader.get_template('all_members.html')
  context = {
    'mymembers': mymembers,
  }
  return HttpResponse(template.render(context, request))

def details(request, id):
  mymember = Member.objects.get(id=id)
  template = loader.get_template('details.html')
  context = {
    'mymember': mymember,
  }
  return HttpResponse(template.render(context, request))

def main(request):
  template = loader.get_template('main.html')
  return HttpResponse(template.render())
```

my_tennis_club/members/urls.py:

```py
from django.urls import path
from . import views

urlpatterns = [
    path('', views.main, name='main'),
    path('members/', views.members, name='members'),
    path('members/details/<int:id>', views.details, name='details'),
]
```

my_tennis_club/members/templates/all_members.html:

```bash
{% extends "master.html" %}

{% block title %}
  My Tennis Club - List of all members
{% endblock %}

{% block content %}

  <p><a href="/">HOME</a></p>

  <h1>Members</h1>

  <ul>
    {% for x in mymembers %}
      <li><a href="details/{{ x.id }}">{{ x.firstname }} {{ x.lastname }}</a></li>
    {% endfor %}
  </ul>
{% endblock %}
```

```py
py manage.py runserver
```

127.0.0.1:8000/:

![007](https://user-images.githubusercontent.com/32337103/215138505-56d25ad0-33d3-480f-8e1f-fbd0092b683c.png)

![008](https://user-images.githubusercontent.com/32337103/215138775-dd6d5698-f1fa-4b48-b117-83e3119df5d2.png)

</details>

<details>
  <summary>20. Customize the 404 Template Page </summary>

- Important: When DEBUG = False, Django requires you to specify the hosts you will allow this Django project to run from.

- In production, this should be replaced with a proper domain name:

ALLOWED_HOSTS = ['yourdomain.com']

- Django will look for a file named 404.html in the templates folder, and display it when there is a 404 error.

- If no such file exists, Django shows the "Not Found" page.

- To customize this message, all you have to do is to create a file in the templates folder and name it 404.html, and fill it with write whatever you want.

my_tennis_club/my_tennis_club/settings.py:

```py
# SECURITY WARNING: don't run with debug turned on in production!
DEBUG = False

ALLOWED_HOSTS = ['*']
```

my_tennis_club/members/templates/404.html:

```html
<!DOCTYPE html>
<html>
  <title>Wrong address</title>
  <body>
    <h1>Ooops!</h1>

    <h2>I cannot find the file you requested!</h2>
  </body>
</html>
```

![008](https://user-images.githubusercontent.com/32337103/215175543-4b34095c-2a20-43f7-9fd9-3ecbcc83f620.png)

</details>

<details>
  <summary>21. Add Django Test View </summary>

my_tennis_club/members/views.py:

```py
from django.http import HttpResponse
from django.template import loader
from .models import Member

def members(request):
  mymembers = Member.objects.all().values()
  template = loader.get_template('all_members.html')
  context = {
    'mymembers': mymembers,
  }
  return HttpResponse(template.render(context, request))

def details(request, id):
  mymember = Member.objects.get(id=id)
  template = loader.get_template('details.html')
  context = {
    'mymember': mymember,
  }
  return HttpResponse(template.render(context, request))

def main(request):
  template = loader.get_template('main.html')
  return HttpResponse(template.render())

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry'],
  }
  return HttpResponse(template.render(context, request))
```

my_tennis_club/members/urls.py:

```py
from django.urls import path
from . import views

urlpatterns = [
    path('', views.main, name='main'),
    path('members/', views.members, name='members'),
    path('members/details/<int:id>', views.details, name='details'),
    path('testing/', views.testing, name='testing'),
]
```

my_tennis_club/members/templates/template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% for x in fruits %}
    <h1>{{ x }}</h1>
    {% endfor %}

    <p>In views.py you can see what the fruits variable looks like.</p>
  </body>
</html>
```

/my_tennis_club

```py
python manage.py runserver
```

127.0.0.1:8000/testing/:

![009](https://user-images.githubusercontent.com/32337103/215180047-35033aa8-cbaa-4063-9344-c1e9580eabf0.png)

</details>

+DJANGO ADMIN

<details>
  <summary>22. Introduction to Django Admin </summary>

```py
py manage.py runserver
```

my_tennis_club/my_tennis_club/urls.py:

```py
from django.contrib import admin
from django.urls import include, path

urlpatterns = [
    path('', include('members.urls')),
    path('admin/', admin.site.urls),
]
```

127.0.0.1:8000/admin/:

![010](https://user-images.githubusercontent.com/32337103/215181307-965a93c3-1826-4fbb-bd20-fa431138fd49.png)

Django Admin - Create User

```py
python manage.py createsuperuser
```

```py
# Username: admin
# Email address: admin@gmail.com
# Password:
# Password (again):
# This password is too short. It must contain at least 8 characters.
# This password is too common.
# This password is entirely numeric.
# Bypass password validation and create user anyway? [y/N]: y

# Superuser created successfully.
```

```py
python manage.py runserver
```

127.0.0.1:8000/admin/:

![010](https://user-images.githubusercontent.com/32337103/215181307-965a93c3-1826-4fbb-bd20-fa431138fd49.png)

![011](https://user-images.githubusercontent.com/32337103/215182500-255292f3-54c8-4952-a79c-9ba658ac8a82.png)

</details>

<details>
  <summary>23. Django Admin - Include Member Model </summary>

- The Members model is missing, as it should be, you have to tell Django which models that should be visible in the admin interface.

- This is done in a file called admin.py, and is located in your app's folder, which in our case is the members folder.

my_tennis_club/members/admin.py:

```py
from django.contrib import admin
from .models import Member

# Register your models here.
admin.site.register(Member)
```

127.0.0.1:8000/admin/:

![011](https://user-images.githubusercontent.com/32337103/215183560-c1d9f4e8-409e-48e9-b564-da01788c9dbd.png)

![012](https://user-images.githubusercontent.com/32337103/215183631-c7dc8b78-bb9e-41ce-8882-1ad9b3c74179.png)

</details>

<details>
  <summary>24. Django Admin - Set Fields to Display </summary>

Make the List Display More Reader-Friendly.

- When you display a Model as a list, Django displays each record as the string representation of the record object, which in our case is "Member object (1)", "Member object(2)" etc.

To change this to a more reader-friendly format, we have two choices:

- Change the string representation function, _str_() of the Member Model.
- Set the list_details property of the Member Model.

To Change the String Representation Function -

my_tennis_club/members/models.py:

```py
from django.db import models

class Member(models.Model):
  firstname = models.CharField(max_length=255)
  lastname = models.CharField(max_length=255)
  phone = models.IntegerField(null=True)
  joined_date = models.DateField(null=True)

  def __str__(self):
    return f"{self.firstname} {self.lastname}"
```

127.0.0.1:8000/admin/:

![](https://user-images.githubusercontent.com/32337103/215197241-8c5136e5-80b9-40f9-a814-0bb81ff6c9d2.png)

To Set list_display -

my_tennis_club/members/admin.py:

```py
from django.contrib import admin
from .models import Member

# Register your models here.

class MemberAdmin(admin.ModelAdmin):
  list_display = ("firstname", "lastname", "joined_date",)

admin.site.register(Member, MemberAdmin)
```

127.0.0.1:8000/admin/:

![](https://user-images.githubusercontent.com/32337103/215197817-cc4a6a91-bc57-48fa-aa18-3cd64ab06eba.png)

</details>

+CONDITIONALS AND OPERATORS

<details>
  <summary>25. Template Variables </summary>

templates/template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>Hello {{ firstname }}, how are you?</h1>

    <p>In views.py you can see how to create the variable.</p>
    <p>In template.html you can see how to use the variable.</p>
  </body>
</html>
```

my_tennis_club/members/views.py:

```py
from django.http import HttpResponse
from django.template import loader
from .models import Member

def members(request):
  mymembers = Member.objects.all().values()
  template = loader.get_template('all_members.html')
  context = {
    'mymembers': mymembers,
  }
  return HttpResponse(template.render(context, request))

def details(request, id):
  mymember = Member.objects.get(id=id)
  template = loader.get_template('details.html')
  context = {
    'mymember': mymember,
  }
  return HttpResponse(template.render(context, request))

def main(request):
  template = loader.get_template('main.html')
  return HttpResponse(template.render())

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'firstname': 'Linus',
  }
  return HttpResponse(template.render(context, request))
```

127.0.0.1:8000/testing/:

![012](https://user-images.githubusercontent.com/32337103/215256961-b62a0903-29f3-4aa0-b953-c202138d280f.png)

Create Variables in Template -

templates/template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% with firstname="Tobias" %}
    <h1>Hello {{ firstname }}, how are you?</h1>
    {% endwith %}
  </body>
</html>
```

my_tennis_club/members/views:

```py
from django.http import HttpResponse
from django.template import loader
from .models import Member

def members(request):
  mymembers = Member.objects.all().values()
  template = loader.get_template('all_members.html')
  context = {
    'mymembers': mymembers,
  }
  return HttpResponse(template.render(context, request))

def details(request, id):
  mymember = Member.objects.get(id=id)
  template = loader.get_template('details.html')
  context = {
    'mymember': mymember,
  }
  return HttpResponse(template.render(context, request))

def main(request):
  template = loader.get_template('main.html')
  return HttpResponse(template.render())

def testing(request):
  template = loader.get_template('template.html')
  return HttpResponse(template.render())
```

127.0.0.1:8000/testing/:

![](https://user-images.githubusercontent.com/32337103/215258927-9de476d0-5a60-48e3-862b-ec3f12aae73f.png)

Data From a Model -

my_tennis_club/members/views.py:

```py
from django.http import HttpResponse
from django.template import loader
from .models import Member

def members(request):
  mymembers = Member.objects.all().values()
  template = loader.get_template('all_members.html')
  context = {
    'mymembers': mymembers,
  }
  return HttpResponse(template.render(context, request))

def details(request, id):
  mymember = Member.objects.get(id=id)
  template = loader.get_template('details.html')
  context = {
    'mymember': mymember,
  }
  return HttpResponse(template.render(context, request))

def main(request):
  template = loader.get_template('main.html')
  return HttpResponse(template.render())

def testing(request):
  mymembers = Member.objects.all().values()
  template = loader.get_template('template.html')
  context = {
    'mymembers': mymembers,
  }
  return HttpResponse(template.render(context, request))

```

templates/template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <ul>
      {% for x in mymembers %}
      <li>{{ x.firstname }}</li>
      {% endfor %}
    </ul>

    <p>
      In views.py you can see how to import and fetch members from the database.
    </p>
  </body>
</html>
```

127.0.0.1:8000/testing/:

![015](https://user-images.githubusercontent.com/32337103/215259182-e501b4c4-4a57-4cc1-a3f9-ecc1e577591a.png)

</details>

<details>
  <summary>26. Django Conditionals and Operators </summary>

If/Else -

templates/template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% if greeting == 1 %}
    <h1>Hello</h1>
    {% else %}
    <h1>Bye</h1>
    {% endif %}

    <p>In views.py you can see what the greeting variable looks like.</p>
  </body>
</html>
```

my_tennis_club/members/views.py:

```py
from django.http import HttpResponse
from django.template import loader
from .models import Member

def members(request):
  mymembers = Member.objects.all().values()
  template = loader.get_template('all_members.html')
  context = {
    'mymembers': mymembers,
  }
  return HttpResponse(template.render(context, request))

def details(request, id):
  mymember = Member.objects.get(id=id)
  template = loader.get_template('details.html')
  context = {
    'mymember': mymember,
  }
  return HttpResponse(template.render(context, request))

def main(request):
  template = loader.get_template('main.html')
  return HttpResponse(template.render())

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'greeting': 1,
  }
  return HttpResponse(template.render(context, request))

```

127.0.0.1:8000/testing/:

![016](https://user-images.githubusercontent.com/32337103/215260865-67cfd700-fb4e-419d-b16c-4f00809c1a9d.png)

If-Elif-Else -

```py
{% if greeting == 1 %}
  <h1>Hello</h1>
{% elif greeting == 2 %}
  <h1>Welcome</h1>
{% else %}
  <h1>Goodbye</h1>
{% endif %}
```

Is equal to -

```py
{% if greeting == 2 %}
  <h1>Hello</h1>
{% endif %}
```

Is not equal to -

```py
{% if greeting != 1 %}
  <h1>Hello</h1>
{% endif %}
```

Is less than -

```py
{% if greeting < 3 %}
  <h1>Hello</h1>
{% endif %}
```

Is less than, or equal to -

```py
{% if greeting <= 3 %}
  <h1>Hello</h1>
{% endif %}
```

Is greater than -

```py
{% if greeting > 1 %}
  <h1>Hello</h1>
{% endif %}
```

Is greater than, or equal to -

```py
{% if greeting >= 1 %}
  <h1>Hello</h1>
{% endif %}
```

And -

```py
{% if greeting == 1 and day == "Friday" %}
  <h1>Hello Weekend!</h1>
{% endif %}
```

Or -

```py
{% if greeting == 1 or greeting == 5 %}
  <h1>Hello</h1>
{% endif %}
```

And/Or -

```py
{% if greeting == 1 and day == "Friday" or greeting == 5 %}
```

In -

```py
{% if 'Banana' in fruits %}
  <h1>Hello</h1>
{% else %}
  <h1>Goodbye</h1>
{% endif %}
```

Not in -

```py
{% if 'Banana' not in fruits %}
  <h1>Hello</h1>
{% else %}
  <h1>Goodbye</h1>
{% endif %}
```

Is -

```py
{% with var1=x var2=x %}
  {% if var1 is var2 %}
    <h1>YES</h1>
  {% else %}
    <h1>NO</h1>
  {% endif %}
{% endwith %}
```

Is not

```py
{% if x is not y %}
  <h1>YES</h1>
{% else %}
  <h1>NO</h1>
{% endif %}
```

</details>

+TEMPLATE TAGS

<details>
  <summary>27. Template Tags - Introduction </summary>

```bs
Tag	            Description

autoescape	    Specifies if autoescape mode is on or off
block	          Specifies a block section
comment	        Specifies a comment section
csrf_token	    Protects forms from Cross Site Request Forgeries
cycle	          Specifies content to use in each cycle of a loop
debug	          Specifies debugging information
extends	        Specifies a parent template
filter	        Filters content before returning it
firstof	        Returns the first not empty variable
for	            Specifies a for loop
if	            Specifies a if statement
ifchanged	      Used in for loops. Outputs a block only if a value has changed since the last iteration
include	        Specifies included content/template
load	          Loads template tags from another library
lorem	          Outputs random text
now	            Outputs the current date/time
regroup	        Sorts an object by a group
resetcycle	    Used in cycles. Resets the cycle
spaceless	      Removes whitespace between HTML tags
templatetag	    Outputs a specified template tag
url	            Returns the absolute URL part of a URL
verbatim	      Specifies contents that should not be rendered by the template engine
widthratio	    Calculates a width value based on the ratio between a given value and a max value
with	          Specifies a variable to use in the block
```

</details>

<details>
  <summary>28. Template Tags - autoescape  </summary>

- The autoescape tag is used to specify if autoescape is on or off.

- If autoescape is on, which is default, HTML code in variables will be escaped.

When escape is on, these characters are escaped:

```bash
< is converted to &lt;
> is converted to &gt;
' is converted to '
" is converted to "
& is converted to &amp;
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% autoescape on %}
    <h1>{{ heading }}</h1>
    {% endautoescape %}

    <p>Check out views.py to see what the heading variable looks like.</p>
  </body>
</html>
```

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'heading': 'Hello &lt;i&gt;my&lt;/i&gt; World!',
  }
  return HttpResponse(template.render(context, request))
```

![](https://user-images.githubusercontent.com/32337103/215270069-1a6fb60f-93f1-438f-87c7-96803a0d2723.png)

</details>

<details>
  <summary>29. Template Tags - block </summary>

The block tag has two functions:

- It is a placeholder for content.
- It is content that will replace the placeholder.

In master templates the block tag is a placeholder that will be replaced by a block in a child template with the same name.<br>

In child templates the block tag is content that will replace the placeholder in the master template with the same name.<br>

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('childtemplate.html')
  return HttpResponse(template.render())

```

mymaster.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>Welcome</h1>

    {% block userinfo %}
    <h2>Not registered yet</h2>
    {% endblock %}

    <p>
      Check out the two templates to see what they look like, and views.py to
      see the reference to the child template.
    </p>
  </body>
</html>
```

childtemplate.html:

```bash
{% extends "mymaster.html" %}

{% block userinfo %}
  <h2>John Doe</h2>
  <p>Explorer of life.</p>
{% endblock %}
```

![](https://user-images.githubusercontent.com/32337103/215270392-c5f022ee-5195-4ff0-8fd5-d6050b6cca89.png)

</details>

<details>
  <summary>30. Template Tags - comment </summary>

- The comment tag allows you to add comment sections that will be ignored by Django.

- Comments can be used to make the code more readable.

- Comments can be used to prevent execution when testing code.

- You can add an explanation to your comments to make them more understandable

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  return HttpResponse(template.render())
```

template.html:

```html
<!DOCTYPE html>
<html>
<body>

<h1>Welcome Everyone!</h1>

{% comment "optional heading" %}
  <h1>Greetings!</h2>
{% endcomment %}

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215273390-bcc5db2d-d576-4ac0-89a7-f9bf4f767132.png)

</details>

<details>
  <summary>31. Template Tags - csrf_token </summary>

views.py:

```py
from django.http import HttpResponse
from django.views.decorators.csrf import csrf_exempt

@csrf_exempt
def my_view(request):
    return HttpResponse('Hello world')
```

template.html:

```html
<!DOCTYPE html>
<html>
  <head> </head>
  <body>
    <form action="" method="post">
      //csrf token inseted in form {% csrf_token %}
      <h2>registration form</h2>
      <input type="text" />
      <input type="submit" />
    </form>
  </body>
</html>
```

</details>

<details>
  <summary>32. Template Tags - cycle </summary>

- The cycle tag returns different values for different iterations in a loop.

- The first iteration gets the first value, the second iteration gets the second value etc.

- You can have as many values as you like.

- If there are more iterations that values, the cycle resets and starts at value 1

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry', 'Orange']
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
<body>

<ul>
{% for x in fruits %}
  <li style='color:{% cycle 'red' 'green' 'blue' 'pink' %}'>
    {{ x }}
  </li>
{% endfor %}
</ul>

<p>Check out views.py to see what the fruits variable looks like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215275833-f39e7516-ba59-43e4-ac65-57e5fc447996.png)

</details>

<details>
  <summary>33. Template Tags - debug	</summary>

Outputs a whole load of debugging information, including the current context and imported modules. {% debug %} outputs nothing when the DEBUG setting is False.

</details>

<details>
  <summary>34. Template Tags - extends </summary>

- The extends tag is used to specify that this template needs a parent template.

- The extends tag takes one argument, which is the name of the parent template.

- When a child template with a parent template is requested, Django uses the parent template as a "skeleton" and fills it with content from the child template, according to the matching block tags.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('childtemplate.html')
  return HttpResponse(template.render())

```

mymaster.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>Welcome</h1>
    <hr />

    {% block heading %}
    <h2>No name</h2>
    {% endblock %}

    <h2>My Cars</h2>

    <ul>
      {% block cars %}
      <li>No cars</li>
      {% endblock %}
    </ul>

    <p>
      Check out the two templates to see what they look like, and views.py to
      see the reference to the child template.
    </p>
  </body>
</html>
```

childtemplate.html:

```bash
{% extends "mymaster.html" %}

{% block heading %}
  <h2>John Doe</h2>
  <p>Explorer of life</p>
{% endblock %}

{% block cars %}
  <li>Ford</li>
  <li>Volvo</li>
  <li>Audi</li>
{% endblock %}
```

![](https://user-images.githubusercontent.com/32337103/215276184-abf815c2-10dc-461f-ae52-6aa96afe3b50.png)

</details>

<details>
  <summary>35. Template Tags - filter </summary>

- The filter tag allows you to run a section of code through a filter, and return it according to the filter keyword(s).

- To add multiple filters, separate the keywords with the pipe | character.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  return HttpResponse(template.render())

```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>Welcome Everyone!</h1>

    {% filter upper %}
    <p>Have a great day!</p>
    {% endfilter %}
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215276359-39aaf01c-6492-453b-a20e-64f9ec2a70db.png)

</details>

<details>
  <summary>36. Template Tags - firstof	 </summary>

- The firstof tag returns the first argument that is not an empty variable.

- Empty variables can be an empty string "", or a zero number 0, or a boolean false.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'x': 'Volvo',
    'y': 'Ford',
    'z': 'BMW',
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>{% firstof x y z %}</h1>

    <p>Check out views.py to see the content of the x, y, and z variables.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215277341-9b630872-fa24-4ad8-bab4-ffe82362e06f.png)

</details>

<details>
  <summary>37. Template Tags - for </summary>

- The for tag allows you to iterate over items in an object.

- Objects can be array-like objects like a Python list or object-like objects like a Python dictionary.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry', 'Orange']
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```HTML
<!DOCTYPE html>
<html>
<body>

<ul>
  {% for x in fruits %}
    <li>{{ x }}</li>
  {% endfor %}
</ul>

<p>Check out views.py to see what the fruits variable looks like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215285954-9eee4f77-0eb0-4eae-90d7-c3a89dfc99c4.png)

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'mycar': {
      'brand': 'Ford',
      'model': 'Mustang',
      'year': '1964',
      }
    }
  return HttpResponse(template.render(context, request))

```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% for x, y in mycar.items %}
    <p>The {{ x }} is {{ y }}.</p>
    {% endfor %}

    <p>Check out views.py to see what the mycar dictionary looks like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215286111-dd9fe999-9eaf-4667-ada9-f49294e3f210.png)

</details>

<details>
  <summary>37a. Template Tags - forloop.counter </summary>

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry', 'Orange']
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <ul>
      {% for x in fruits %}
      <li>{{ forloop.counter }}</li>
      {% endfor %}
    </ul>

    <p>Check out views.py to see what the fruits object look like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215287416-5d42c636-5d6f-4640-b8a8-30f4f6ea4dae.png)

</details>

<details>
  <summary>37b. Template Tags - forloop.counter0 </summary>

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry', 'Orange']
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <ul>
      {% for x in fruits %}
      <li>{{ forloop.counter0 }}</li>
      {% endfor %}
    </ul>

    <p>Check out views.py to see what the fruits object look like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215287625-7515c4e2-0452-4e9a-af28-eb88d5c53938.png)

</details>

<details>
  <summary>37c. Template Tags - forloop.first </summary>

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry', 'Orange']
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```py
<!DOCTYPE html>
<html>
<body>

<ul>
  {% for x in fruits %}
    <li
    {% if forloop.first %}
      style='background-color:lightblue;'
    {% endif %}
    >{{ x }}</li>
  {% endfor %}
</ul>

<p>Check out views.py to see what the fruits object look like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215287969-9f101f82-519c-4fed-987f-90d65d3165ca.png)

</details>

<details>
  <summary>37d. Template Tags - forloop.last </summary>

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry', 'Orange']
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <ul>
      {% for x in fruits %}
      <li {% if forloop.last %} style="background-color:lightblue;" {% endif %}>
        {{ x }}
      </li>
      {% endfor %}
    </ul>

    <p>Check out views.py to see what the fruits object look like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215288123-0a77085f-9afb-4ddd-83ab-c5556cc8c3d8.png)

</details>

<details>
  <summary>37e. Template Tags - forloop.parentloop </summary>

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'cars': ['Ford', 'Volvo', 'BMW'],
    'colors': ['Red', 'Green', 'Blue']
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```py
<!DOCTYPE html>
<html>
<body>

<ul>
  {% for x in cars %}
    <li>{{ x }}:
      <ul>
        {% for y in colors %}
          <li>
            {{ forloop.parentloop.counter }}
            {{ y }}
          </li>
        {% endfor %}
      </ul>
    </li>
  {% endfor %}
</ul>

<p>Check out views.py to see what the cars and colors object look like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215288312-62fababe-ecec-4fc2-b54f-463752e525c4.png)

</details>

<details>
  <summary>37f. Template Tags - forloop.revcounter </summary>

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry', 'Orange']
    }
  return HttpResponse(template.render(context, request))

```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <ul>
      {% for x in fruits %}
      <li>{{ forloop.revcounter }}</li>
      {% endfor %}
    </ul>

    <p>Check out views.py to see what the fruits object look like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215288555-6dd476a2-0c7a-423b-9bcf-b4949c288134.png)

</details>

<details>
  <summary>37g. Template Tags - forloop.revcounter0 </summary>

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry', 'Orange']
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```py
<!DOCTYPE html>
<html>
<body>

<ul>
  {% for x in fruits %}
    <li>{{ forloop.revcounter }}</li>
  {% endfor %}
</ul>

<p>Check out views.py to see what the fruits object look like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215288704-6c62f5ad-9c1c-4b6e-85a2-4db3cfe4bf4b.png)

</details>

<details>
  <summary>38. Template Tags - if </summary>

- The if tag allows you to write conditional statements.

- Use if statements to output a block of code if a condition is true.

- You can use else or elif (short for "else if") to specify what to do when the if condition is false.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'myvar': 1
    }
  return HttpResponse(template.render(context, request))

```

template.html:

```py
<!DOCTYPE html>
<html>
<body>

{% if myvar == 1 %}
  <h1>Hello!</h1>
{% endif %}

<p>Check out views.py to see what the myvar variable looks like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215289374-01ae974d-64c2-4fb9-865c-5567c4b70454.png)

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'myvar': 2
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```py
<!DOCTYPE html>
<html>
<body>

{% if myvar == 1 %}
  <h1>Hello!</h1>
{% elif myvar == 2 %}
  <h1>Welcome!</h1>
{% else %}
  <h1>Greetings!</h1>
{% endif %}

<p>Check out views.py to see what the myvar variable looks like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215290382-596fa475-3e4f-4a51-8ec6-dc2795e7d337.png)

</details>

<details>
  <summary>39. Template Tags - ifchanged </summary>

- The ifchanged tag allows you to check a value in a loop and output a code if the value has changed since the last iteration.

- If the iteration object has many values per iteration, you can specify which value to check, and the block of code will only displayed if that value has changed since the last iteration.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'mylist': [1, 1, 1, 2, 2, 2, 2, 3, 3, 3, 3, 4, 5]
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```bash
<!DOCTYPE html>
<html>
<body>

<ul>
  {% for x in mylist %}
    {% ifchanged %}
      <li>{{ x }}</li>
    {% endifchanged %}
  {% endfor %}
</ul>

<p>Check out views.py to see what the mylist object look like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215290542-2a80c3b1-625f-4077-b188-6cb41563102c.png)

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'cars': [
      {
        'brand': 'Ford',
        'model': 'Mustang',
        'year': '1964',
      },
      {
        'brand': 'Ford',
        'model': 'Bronco',
        'year': '1970',
      },
      {
        'brand': 'Ford',
        'model': 'Sierra',
        'year': '1981',
      },
      {
        'brand': 'Volvo',
        'model': 'XC90',
        'year': '2016',
      },
      {
        'brand': 'Volvo',
        'model': 'P1800',
        'year': '1964',
      }]
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% for x in cars %} {% ifchanged x.brand %}
    <h1>{{ x.brand }}:</h1>
    {% endifchanged %}
    <p>{{ x.model }}, {{ x.year }}</p>
    {% endfor %}

    <p>Check out views.py to see what the cars object look like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215290655-dedf12cf-f8af-4c09-bc34-53a7b0e9aed4.png)

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'mylist': [1, 1, 1, 2, 2, 2, 2, 3, 3, 3, 3, 4, 5]
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```py
<!DOCTYPE html>
<html>
<body>

{% for x in mylist %}
  {% ifchanged %}
    <p>New value: {{ x }}</p>
  {% else %}
    <p>Same value: {{ x }}</p>
  {% endifchanged %}
{% endfor %}

<p>Check out views.py to see what cars object look like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215291268-3f5646a2-5cf9-4825-8dd3-78ddd1694353.png)

</details>

<details>
  <summary>40. Template Tags - include </summary>

- The include tag allows you to include content from another template.

- Place the include tag exactly where you want the content to be displayed.

- This is useful when you have the same content for many pages.

- You can also send variables into the template, by using the with keyword.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  return HttpResponse(template.render())
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% include "mymenu.html" with me="ALEXANDER" sponsor="W3SCHOOLS" %}

    <h1>Welcome</h1>

    <p>This is my web site.</p>

    <p>Check out mymenu.html to see the HTML content of the include.</p>
  </body>
</html>
```

mymenu.html:

```html
<div>HOME | {{ me }} | ABOUT | FORUM | {{ sponsor }}</div>
```

![](https://user-images.githubusercontent.com/32337103/215291493-d86a684c-a81c-44b6-948f-8c10b52415c4.png)

</details>

<details>
  <summary>41. Template Tags - load </summary>

Loads template tags from another library.

```py

```

</details>

<details>
  <summary>42. Template Tags - lorem  </summary>

- The lorem tag inserts a specified amount of random text.

- The "random" text is the famous "Lorum ipsum" text, in lower case letters.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  return HttpResponse(template.render())
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% lorem 50 w %}
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215291751-4f1e3f19-4c58-4647-bf8a-2f164dbf26f5.png)

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% lorem 5 p %}
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215291835-de7e51f7-a543-4a4d-b646-4a20f56d8b76.png)

```py
{% lorem count method random %}
```

</details>

<details>
  <summary>43. Template Tags - now </summary>

The now tag inserts the current date and/or time, according to the specified format.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  return HttpResponse(template.render())
```

template.html:

```py
<!DOCTYPE html>
<html>
<body>

<h1>{% now "Y-m-d G:i:s" %}</h1>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215291958-ecc2a2d3-2960-4c12-ad6c-f99b0f18ab3b.png)

```py
{% now format %}
```

</details>

<details>
  <summary>44. Template Tags - regroup </summary>

- The regroup tag returns a new object grouped by a specified value.

- The result is divided into one GroupedResult object for each group, making the newlist object.

- Make sure the object is sorted correctly before regrouping, otherwise you will end up with groups with the same grouper name.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'cars': [
      {
        'brand': 'Ford',
        'model': 'Mustang',
        'year': '1964',
      },
      {
        'brand': 'Ford',
        'model': 'Bronco',
        'year': '1970',
      },
      {
        'brand': 'Ford',
        'model': 'Sierra',
        'year': '1981',
      },
      {
        'brand': 'Volvo',
        'model': 'XC90',
        'year': '2016',
      },
      {
        'brand': 'Volvo',
        'model': 'P1800',
        'year': '1964',
      }]
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% regroup cars by brand as newlist %} {{ newlist }} {% for x in newlist %}
    <h1>{{ x.grouper }}</h1>
    {% for y in x.list %}
    <p>{{ y.model }}: {{ y.year }}</p>
    {% endfor %} {% endfor %}

    <p>Check out views.py to see what the cars list looks like.</p>
  </body>
</html>
```

The result from {% regroup cars by brand as newlist %}:

```py
[
  GroupedResult(
    grouper='Ford',
    list=[
      {
        'brand': 'Ford',
        'model': 'Mustang',
        'year': '1964'
      },
      {
        'brand': 'Ford',
        'model': 'Bronco',
        'year': '1970'
      },
      {
        'brand': 'Ford',
        'model': 'Sierra',
        'year': '1981'
      }
    ]
  ),
  GroupedResult(
    grouper='Volvo',
    list=[
      {
        'brand': 'Volvo',
        'model': 'XC90',
        'year': '2016'
      },
      {
        'brand': 'Volvo',
        'model': 'P1800',
        'year': '1964'
      }
    ]
  )
]
```

![](https://user-images.githubusercontent.com/32337103/215292099-a778f455-c480-45ed-b391-3d942d0e4fc5.png)

```py
{% regroup object by object.property as newname %}
```

</details>

<details>
  <summary>45. Template Tags - resetcycle </summary>

- The resetcycle tag is used inside a cycle, and resets the cycle, making it start at the beginning.

- It does not reset the loop, only the cycle.

- If you have multiple cycles, you can specify which one to reset with the name argument.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry', 'Orange']
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
<body>

<ul>
  {% for x in fruits %}
    <li style='color:{% cycle 'red' 'green' 'blue' 'pink' %}'>
      {{ x }}
    </li>
    {% if x == "Banana" %}
      {% resetcycle %}
    {% endif %}
  {% endfor %}
</ul>

<p>Check out views.py to see what the fruits variable looks like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215292269-bde32742-f152-46f3-ac8c-b2a8422e54ad.png)

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry', 'Orange']
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
<body>

<ul>
{% for x in fruits %}
  <li style='
      color:{% cycle 'red' 'green' 'blue' 'pink' as mycolor %};
      background:{% cycle 'grey' 'beige' 'red' 'purple' as mybg %};
    '>
    {{ x }}
  </li>
  {% if x == "Banana" %}
    {% resetcycle mybg %}
  {% endif %}
{% endfor %}
</ul>

<p>Check out views.py to see what the fruits variable looks like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215292325-82fc7cab-dbc2-445b-a96b-d974a790f3ea.png)

</details>

<details>
  <summary>46. Template Tags - spaceless </summary>

- The spaceless tag is used to remove any space between tags, in the code.

- The spaceless tag removes any whitespaces, new lines and tabs.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry', 'Orange']
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% spaceless %}
    <ul>
      {% for x in fruits %}
      <li>{{ x }}</li>
      {% endfor %}
    </ul>
    {% endspaceless %}

    <p>
      Right-click the result and view the page source. The entire HTML code is
      written in one line.
    </p>

    <p>Check out views.py to see what the fruits variable looks like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215292391-dbc43074-3a56-48d3-996b-a9941b0b358e.png)

</details>

<details>
  <summary>47. Template Tags - templatetag </summary>

- The templatetag tag is used to display characters that are normally used to perform Django tasks.

- Each tag character, like {{, {% and {#, has their own name.

```bash
Name	          Output
openvariable	  {{
closevariable	  }}
openblock	      {%
closeblock	    %}
openbrace	      {
closebrace	    }
opencomment	    {#
closecomment	  #}
```

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  return HttpResponse(template.render())
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>{% templatetag openblock %} extends {% templatetag closeblock %}</h1>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215292512-f1b80172-ca7b-4e80-89d6-1955784d8e12.png)

</details>

<details>
  <summary>48. Template Tags - url </summary>

Returns the absolute URL part of a URL.

```py
{% url login.views.login_view %}
```

</details>

<details>
  <summary>49. Template Tags - verbatim </summary>

- The verbatim tag is used to stop Django from executing code.

- Anything between {% verbatim %} and {% endverbatim %} will not be executed, but rendered as output instead.

- To be sure that you refer to the correct verbatim code block, you can add a name to it:

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry', 'Orange']
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```py
<!DOCTYPE html>
<html>
<body>

{% verbatim %}
  {% for x in fruits %}
    <h1>{{ x }}</h1>
  {% endfor %}
{% endverbatim %}

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215292811-2cf341ef-6139-4edc-b808-ec89c7cb2966.png)

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% verbatim mycode %} {% for x in fruits %} {% verbatim %}
    <h1>{{ x }}</h1>
    {% endverbatim %} {% endfor %} {% endverbatim mycode %}
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215292853-5ce3a378-5453-4145-80fe-9f41f63bda0c.png)

</details>

<details>
  <summary>50. Template Tags - widthratio </summary>

Calculates a width value based on the ratio between a given value and a max value.

```py

```

</details>

<details>
  <summary>A51. Template Tags - with  </summary>

- The with tag is used to create variables in Django templates.

- This can be useful when you need to ask for the same variable many times, like in a loop.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  return HttpResponse(template.render())
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% with firstname="Stalikken" %}
    <h1>Hello {{ firstname }}</h1>
    {% endwith %}
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215292934-de95c829-2e36-4af1-8844-a5f539e8849a.png)

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry', 'Orange']
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```code
<!DOCTYPE html>
<html>
<body>

{% with myvar=fruits|length %}
  {% for x in fruits %}
     <p>{{ x }} is one of {{ myvar }} fruits.</p>
  {% endfor %}
{% endwith %}

<p>Check out views.py to see what the fruits list looks like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215292976-99312dc9-935f-4ac7-ba58-4ff299544421.png)

</details>

<details>
  <summary>52. Template Tags - Reversed keyword </summary>

The reversed keyword is used when you want to do the loop in reversed order.

views.py:

```py
from django.http import HttpResponse, HttpResponseRedirect
from django.template import loader
from .models import Member

def testing(request):
  mymembers = Member.objects.all().values()
  template = loader.get_template('template.html')
  context = {
    'members': mymembers,
  }
  return HttpResponse(template.render(context, request))

```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% for x in members reversed %}
    <h1>{{ x.id }}</h1>
    <p>{{ x.firstname }} {{ x.lastname }}</p>
    {% endfor %}

    <p>
      In views.py you can see how to import and fetch members from the database.
    </p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215293203-bd6a067c-660a-479d-8cad-72e8b12a9cb7.png)

</details>

<details>
  <summary>53. Template Tags - Empty keyword </summary>

- The empty keyword can be used if you want to do something special if the object is empty.

- The empty keyword can also be used if the object does not exist.

views.py:

```py
from django.http import HttpResponse, HttpResponseRedirect
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'emptytestobject': [],
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <ul>
      {% for x in emptytestobject %}
      <li>{{ x.firstname }}</li>
      {% empty %}
      <li>No members</li>
      {% endfor %}
    </ul>

    <p>In views.py you can see the emptytestobject.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215293477-65d7ce47-d730-4328-9b1f-24235855825a.png)

views.py:

```py
from django.http import HttpResponse, HttpResponseRedirect
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry'],
  }
  return HttpResponse(template.render(context, request))

```

template.html:

```py
<!DOCTYPE html>
<html>
<body>

<ul>
  {% for x in myobject %}
    <li>{{ x.firstname }}</li>
  {% empty %}
    <li>No members</li>
  {% endfor %}
</ul>

<p>In views.py you can see that there is no myobject variable.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215293538-b2cdcb56-df37-4cb3-ac6e-b778cc7490b4.png)

</details>

<details>
  <summary>54. Template Tags - Comments </summary>

- Comments allows you to have sections of code that should be ignored.

- You can add a message to your comment, to help you remember why you wrote the comment, or as message to other people reading the code.

- You can also use the {# ... #} tags when commenting out code, which can be easier for smaller comments.

- Views are written in Python, and Python comments are written with the # character.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  return HttpResponse(template.render())
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>Welcome Everyone</h1>
    {% comment %}
    <h1>Welcome ladies and gentlemen</h1>
    {% endcomment %}
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215293655-e05a591b-333f-43b4-9178-e78940ec2048.png)

```html
<h1>Welcome Everyone</h1>
{% comment "this was the original welcome message" %}
<h1>Welcome ladies and gentlemen</h1>
{% endcomment %}
```

```html
<h1>Welcome{# Everyone#}</h1>
```

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  #context = {
  # 'var1': 'John',
  #}
  return HttpResponse(template.render())
```

</details>

<details>
  <summary>55. Template Tags - Include </summary>

- The include tag allows you to include a template inside the current template.

- This is useful when you have a block of content that is the same for many pages.

- You can send variables into the template by using the with keyword.

- In the include file, you refer to the variables by using the {{ variablename }} syntax.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  return HttpResponse(template.render())
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>Hello</h1>

    <p>This page contains a footer in a template.</p>

    {% include 'footer.html' %}

    <p>
      Check out the two templates to see what they look like, and views.py to
      see the reference to the child template.
    </p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215293916-0331fa94-ed0e-4c9d-a137-7afbb16594c5.png)

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  return HttpResponse(template.render())

```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% include "mymenu.html" with me="TOBIAS" sponsor="W3SCHOOLS" %}

    <h1>Welcome</h1>

    <p>This is my web site.</p>

    <p>Check out mymenu.html to see the HTML content of the include.</p>
  </body>
</html>
```

mymenu.html:

```py
<div>HOME | {{ me }} | ABOUT | FORUM | {{ sponsor }}</div>
```

![](https://user-images.githubusercontent.com/32337103/215293994-22060211-83c7-41ce-bd51-4adf2372bf0c.png)

</details>

+FILTER REFERENCE

<details>
  <summary>56. Filter Reference - add </summary>

- The add filter adds a specified argument to a value.

- The add filter tries to convert the values into numbers and return the sum, but if is not possible to convert the values into numbers, the specified argument will be added at the end.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'prices': [70, 35, 52],
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% for x in prices %}
    <h1>The price is {{ x|add:"10" }} dollars.</h1>
    {% endfor %}

    <p>In views.py you can see what the prices variable looks like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215329917-31ca505c-7882-4b94-b4db-4b97fc307bf8.png)

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry'],
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```py
<!DOCTYPE html>
<html>
<body>

{% for x in fruits %}
  <h1>{{ x|add:"-CHECK" }}</h1>
{% endfor %}

<p>In views.py you can see what the fruits variable looks like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215330058-4f1f81ab-b653-4bf2-b5e6-25fc066c2296.png)

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry'],
    'vegetables': ['Asparagus', 'Broccoli', 'Carrot'],
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```py
<!DOCTYPE html>
<html>
<body>

{{ fruits|add:vegetables }}

<p>In views.py you can see what the fruits
and vegetables variables look like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215330188-5b8131da-d03a-40a3-bccb-c19d54edda37.png)

</details>

<details>
  <summary>57. Filter Reference - addslashes </summary>

- The addslashes filter adds a slash \ character before any quotes.

- This can be helpful when you are dealing with JavaScript, and you have to escape quote characters.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'name': "Capt'n Jack",
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>{{ name|addslashes }}</h1>

    <p>In views.py you can see what the name variable looks like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215330828-5a372836-3cdb-41b7-a280-3e048161404f.png)

</details>

<details>
  <summary>58. Filter Reference - capfirst </summary>

The capfirst filter capitalizes the first letter of the value.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'animal': 'lion',
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>{{ animal|capfirst }}</h1>

    <p>In views.py you can see what the animal variable looks like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215331045-40a87606-e020-4e1e-ba55-c61d4a65840e.png)

</details>

<details>
  <summary>59. Filter Reference - center </summary>

The center filter places the value in the center of a value of the specified length.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'name': 'Tobias',
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>{{ name|center:20 }}</h1>

    <p>
      In HTML the display does not show more than one space, but if you view the
      page source you will see that there are 20 characters between &lt;h1&gt;
      and &lt;/h1&gt;.
    </p>

    <p>
      Or, to demonstrate we can use a textarea to see that "Tobias" is center
      aligned:
    </p>

    <textarea>{{ name|center:20 }}</textarea>

    <p>In views.py you can see what the name variable looks like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215331340-2a3a1963-0686-44bd-bb14-10a215a3982d.png)

</details>

<details>
  <summary>60. Filter Reference - cut </summary>

- The cut filter removes the specified phrase from the value.

- The cut filter is case sensitive.

- All occurences of the specified phrase/character are removed.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'name': 'Emil Refsnes',
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>{{ name|cut:"snes" }}</h1>

    <p>In views.py you can see what the name variable looks like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215331712-6c51ca13-a1aa-4290-a16f-b006dc2dc5b0.png)

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'name': 'Emil Refsnes',
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>{{ name|cut:"e" }}</h1>

    <p>In views.py you can see what the name variable looks like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215331793-64c3a751-c631-4463-bf48-4a6c822afc57.png)

</details>

<details>
  <summary>61. Filter Reference - default </summary>

- The default filter allows you to specify a default value to use if the value evaluates to False.

Values that evaluates to False are:

- Empty Strings ""
- Any numeric 0
- Any empty object [], (), {}, set(), range(0)
- None
- False

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'colors': ['Red', 'Green', 'Blue', '', 'Yellow']
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% for x in colors %}
    <h1>{{ x|default:"nocolor" }}</h1>
    {% endfor %}

    <p>In views.py you can see what the colors variable looks like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215332377-323885df-93f8-45b8-bf0f-e06a828a575b.png)

</details>

<details>
  <summary>62. Filter Reference - default if none </summary>

- The default_if_none filter allows you to specify a default value to use if the value is None.

- The value has to be exactly None for this filter to have effect.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'colors': ['Red', None, 'Blue', '', 'Yellow']
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```py
<!DOCTYPE html>
<html>
<body>

{% for x in colors %}
  <h1>{{ x|default_if_none:"nocolor" }}</h1>
{% endfor %}

<p>In views.py you can see what the colors variable looks like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215332945-19576437-2c74-4c2d-9b39-774d585609f1.png)

</details>

<details>
  <summary>63. Filter Reference - dictsort </summary>

- The dictsort filter sorts a dictionary by the specified field.

- The dictsort filter sorts ascending.

- Use the dictsortreversed filter to sort descending.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'cars': [
      {'brand': 'Ford', 'model': 'Mustang', 'year': 1964},
      {'brand': 'Volvo', 'model': 'XC90', 'year': 2022},
      {'brand': 'Volvo', 'model': 'P1800', 'year': 1962},
      {'brand': 'Ford', 'model': 'Focus', 'year': 2004},
    ]
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```py
<!DOCTYPE html>
<html>
<body>

{% for x in cars|dictsort:"year" %}
  <p>{{ x.year }} {{ x.brand }} {{ x.model }}.</p>
{% endfor %}

<p>In views.py you can see what the colors variable looks like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215333363-4679cb6d-0fe7-454e-ac27-423d13e0d974.png)

</details>

<details>
  <summary>64. Filter Reference - dictsortreversed </summary>

- The dictsortreversed filter sorts a dictionary by the specified field, descending.

- Use the dictsort filter to sort ascending.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'cars': [
      {'brand': 'Ford', 'model': 'Mustang', 'year': 1964},
      {'brand': 'Volvo', 'model': 'XC90', 'year': 2022},
      {'brand': 'Volvo', 'model': 'P1800', 'year': 1962},
      {'brand': 'Ford', 'model': 'Focus', 'year': 2004},
    ]
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    {% for x in cars|dictsortreversed:"year" %}
    <p>{{ x.year }} {{ x.brand }} {{ x.model }}.</p>
    {% endfor %}

    <p>In views.py you can see what the colors variable looks like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215334222-18ee4b35-c15a-4796-b938-1cc8c6f0a2fe.png)

</details>

<details>
  <summary>65. Filter Reference - divisibleby </summary>

The divisibleby filter returns True if the value is divisible by the argument, otherwise it returns False.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'totalsum': 40,
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```py
<!DOCTYPE html>
<html>
<body>

{% if totalsum|divisibleby:5 %}
  <h1>Yes, it is!</h1>
{% endif %}

<p>In views.py you can see what the totalsum variable looks like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215334771-4988bd47-1514-46d1-9bfd-afc6c367a7b4.png)

</details>

<details>
  <summary>66. Filter Reference - escape </summary>

The escape filter escapes HTML characters from the value.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'heading': 'Hello &lt;i>my&lt;/i> World!',
  }
  return HttpResponse(template.render(context, request))
```

```html
<!DOCTYPE html>
<html>
  <body>
    {% autoescape off %}
    <h1>{{ heading|escape }}</h1>
    <h1>{{ heading }}</h1>
    {% endautoescape %}

    <p>In views.py you can see what the heading variable looks like.</p>

    <p>
      <strong>Note:</strong>
      Escaping HTML characters is a default setting in Django, so we have to
      turn off autoescape in the example to see the difference.
    </p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215335205-da51b744-0cb1-4f7a-a4aa-d8c10caa0f12.png)

</details>

<details>
  <summary>67. Filter Reference - escapejs </summary>

The escapejs filter escapes text to be used in JavaScript strings.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'var1': 'John\nDoe',
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h3>Without escapejs:</h3>
    <button onclick="alert('{{ var1 }}')">Click me</button>

    <h3>With escapejs:</h3>
    <button onclick="alert('{{ var1|escapejs }}')">Click me</button>

    <p>
      Try clicking both buttons. The JavaScript without the escapejs filter will
      raise an error.
    </p>

    <p>In views.py you can see what the var1 variable looks like.</p>
  </body>
</html>
```

</details>

<details>
  <summary>68. Filter Reference - filesizeformat </summary>

- The filesizeformat filter converts a large number into a more human readable format.

Examples:

- 1024 is converted into 1.0 KB.

- 524288 is converted into 512.0 KB.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'size': 26214400
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```py
<!DOCTYPE html>
<html>
<body>

<h1>{{ size|filesizeformat }}</h1>

<p>In views.py you can see what the size variable looks like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215335665-dd213300-acd1-478a-9f40-e6dbbc671eb1.png)

</details>

<details>
  <summary>69. Filter Reference - first </summary>

- The first filter returns the first item of an object.

- For strings, the first filter returns the first character.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry', 'Orange']
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>{{ fruits|first }}</h1>

    <p>In views.py you can see what the fruits variable looks like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215335849-f19ea176-b87b-4704-a7e4-27625e012486.png)

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'firstname': 'Emil',
    'lastname': 'Refsnes',
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>{{ firstname|first }}</h1>

    <p>In views.py you can see what the firstname variable looks like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215335911-fba4513b-0462-4bae-9aaf-5e95d55eb919.png)

</details>

<details>
  <summary>70. Filter Reference - floatformat </summary>

- The floatformat filter rounds a floating-point number to the specified number of decimals, or one, if no decimal argument is specified.

- If the argument value is a positive number, the value will be displayed with the specified number of decimals, even if the value is an integer.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'mynumber': 7.122489,
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>{{ mynumber|floatformat:2 }}</h1>

    <p>In views.py you can see what the mynumber variable looks like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215336012-5bc68756-d58b-4482-a4c9-8b0bb885c039.png)

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  return HttpResponse(template.render())
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <p>{{ 7.122489|floatformat:2 }}</p>
    <p>{{ 7.1|floatformat:2 }}</p>
    <p>{{ 7|floatformat:2 }}</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215336096-8601e42d-31d6-42b8-9ff7-e48bc6ee1856.png)

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  return HttpResponse(template.render())
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <p>{{ 7.122489|floatformat:-2 }}</p>
    <p>{{ 7.1|floatformat:-2 }}</p>
    <p>{{ 7|floatformat:-2 }}</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215336338-8c072038-44e3-4281-8815-be0c85a72122.png)

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  return HttpResponse(template.render())
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <p>{{ 7.122489|floatformat:-2 }}</p>
    <p>{{ 7.1|floatformat:-2 }}</p>
    <p>{{ 7|floatformat:-2 }}</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215336425-a1d7acf2-d1fe-4dd5-bd42-dc9061b68f43.png)

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'mynumber': 981358286,
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```py
<!DOCTYPE html>
<html>
<body>

<h1>{{ mynumber|floatformat:"2g" }}</h1>

<p>In views.py you can see what the mynumber variable looks like.</p>

</body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215336543-ade9c2e7-9caf-4215-8e86-3ddb5d32684d.png)

</details>

<details>
  <summary>71. Filter Reference - get_digit </summary>

The get_digit filter returns the specified digit from a number, counting from the end of the number.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'mynumber': 75641,
  }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>{{ mynumber|get_digit:2 }}</h1>

    <p>In views.py you can see what the mynumber variable looks like.</p>
  </body>
</html>
```

![](https://user-images.githubusercontent.com/32337103/215336894-da367535-4fe5-41dc-986f-098f5ec4400f.png)

</details>

<details>
  <summary>72. Filter Reference - join </summary>

- The join filter takes all items in an iterable and joins them into one string.

- A string must be specified as the separator.

views.py:

```py
from django.http import HttpResponse
from django.template import loader

def testing(request):
  template = loader.get_template('template.html')
  context = {
    'fruits': ['Apple', 'Banana', 'Cherry', 'Orange']
    }
  return HttpResponse(template.render(context, request))
```

template.html:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>{{ fruits|join:"#" }}</h1>

    <p>In views.py you can see what the fruits variable looks like.</p>
  </body>
</html>
```

</details>

<details>
  <summary>73. Filter Reference - join_script </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>74. Filter Reference - last </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>75. Filter Reference - length </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>76. Filter Reference - length_js </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>77. Filter Reference - linebreaks </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>78. Filter Reference - linebreaksbr </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>79. Filter Reference - linenumbers </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>80. Filter Reference - ljust </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>81. Filter Reference - lower </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>82. Filter Reference - make_list </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>83. Filter Reference - phone2numeric </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>84. Filter Reference - pluralize </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>85. Filter Reference - random </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>86. Filter Reference - rjust </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>87. Filter Reference - slice </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>88. Filter Reference - slugify </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>89. Filter Reference - striptags </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>90. Filter Reference - time </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>91. Filter Reference - timesince </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>92. Filter Reference - timeuntil </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>93. Filter Reference - title </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>94. Filter Reference - title </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>95. Filter Reference - truncatechars </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>96. Filter Reference - truncatechars_html </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>97. Filter Reference - truncatewords </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>98. Filter Reference - truncatewords_html </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>99. Filter Reference - unordered_list </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>100. Filter Reference - upper </summary>

```py

```

```py

```

```py

```

```py

```

</details>
