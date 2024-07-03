# Basic intro to python

| This lesson will use 3 main file, main.py, main2.py and main3.py, go in order

(Make sure to view this file in reading mode, click buttons in top right until a preview opens.)

**Now to the lesson**

The first task will be to print a string multiple times in a row, you can do this in main.py


Done? Cool, click below

<details>
 <summary>Answer (click me)</summary>
 Your code should have print "Hello World!" 10 times

   Console Output

   ```
   Hello World!
   Hello World!
   Hello World!
   Hello World!
   Hello World!
   Hello World!
   Hello World!
   Hello World!
   Hello World!
   Hello World!
   Complete
   ```

   Code:
 
   ```python
   for i in range(10):
     print("Hello World!")
   ```

</details>


#

**Lesson 1 pt 2**

In this part we will use functions and maths in python

Example function :
```python
# Define the function
def print_v2(text1, text2):
    print(text1)
    print(text2)

# Call the function
print_v2("Hello World v1", "Hello World v2")

# End
```
Output:
```
Hello World v1
Hello World v2
```

Now your task, open main2.py and go through the lesson there

<details>
 <summary>Hint (click me)</summary>

Python Maths:
```
Addition = +

Subtraction = -

Multiplication = *

Division = /
```

</details>
<details>
 <summary>Answer (click me)</summary>

 Console Output:

 ```
 6
 2
 24
 1.5
 ```

 Python Code:
 ```python
 # Setup variables
var1 = 6
var2 = 4

# Define Function
def maths(var1, var2):
    print(var1 + var2)
    print(var1 - var2)
    print(var1 * var2)
    print(var1 / var2)

# use the function (example: maths_function(var1, var2))
maths(var1, var2)

```
</details>

```python
# One thing you can do is add values to a variable

# Define the function
number = 5

# Add 3 to the number
number += 3

# Print the new number
print(number)

# Would print 8
```
#

**Lesson 1 pt 3**

In this part we will be making variables using functions in python

Basic example:
```python
# Define the function
def get_text():
    return "Hello World! This is a basic function!"

# Call the function
text = get_text()
print(text)

# Another method is just directly printing the function value
print(get_text())
```

Output:
```
Hello World! This is a basic function!
Hello World! This is a basic function!
```

__Cool Info__

You can define 2 variables with different values in one function. It is done like this:

```python
# Define the function
def get_text_and_number():
    return "Hello World!", 7

# Call the function
text, number = get_text_and_number()
print(text)
print(number)
```

Output:
```
Hello World!
7
```

__Now your turn__

Go to main3.py and complete the lesson in there.

<details>
 <summary>Answers (click me)</summary>

 Console Output:
 ```
 Hello World! Basic Function!
 Cool
 174

 (If u did the challange):
 Hello World! Basic Function!Cool
 ```

 Python Code:
 ```python
# Define the first function
def get_string():
    return "Hello World! Basic Function!"

# Define the second function
def get_string_and_int():
    return "Cool", 174

# Call the first function a print the value
print(get_string())

# Call the second function and print the two values
text, number = get_string_and_int()
print(text)
print(number)

# Challange:
# Print the text values of both functions in one line:
print(get_string() + get_string_and_int()[0])

# Also a valid way
print(get_string() + text)
```

</details>
