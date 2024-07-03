# User Controlled Programs

**Lesson 2 pt 1**

In this part we will be making a user controlled program in python

This will involve getting input from the user, user choosing where they want to go in the program, and handling that input.

Basic input example:
```python
# Get the users favorite number in string form
fav_num = input("What is your favorite number? ")
# Print the users favorite number
print("Cool, your favorite number is " + fav_num)

# Get the users favorite number in int form
fav_num = int(input("What is your favorite number? "))
# Print the users favorite number
print("Cool, your favorite number is " + str(fav_num))
```

To handle that data we will use an `if` statement.

Example:
```python
# Get the users favorite number in int form
fav_num = int(input("What is your favorite number? "))
# Print the users favorite number
if fav_num > 10:
    print("Your favorite number is greater than 10")
# Elif statement combinse else and if statement
elif fav_num == 10:
    print("Your favorite number is 10")
else:
    print("Your favorite number is less than 10")
```

**Now your turn to code!**

Go to main.py and complete the task in there

<details>
<summary>Answers</summary>

Console Output:

```
How old are you: 10
Your age is 10
```

Python Code:
```python
# Get the users age
age = int(input("How old are you: "))
or
age = input("How old are you: ")

# Print the users age
print("Your age is " + str(age))
```

</details>

#

**Lesson 2 pt 2**

In this part we will be comparing strings in python

You are able to compare strings in python like you compare numbers

Example:
```py
# Define the two strings
string1 = "k"
string2 = "h"

# Compare the two strings
if string1 < string2:
    print(f"{string1} is less than {string2}")
elif string1 == string2:
    print(f"{string1} is equal to {string2}")
else:
    print(f"{string1} is greater than {string2}")
```

**Now your turn to code!**

Go to main2.py and complete the task in there :D

<details>
 <summary>Answers</summary>

 Python Code:
 ```python
# Ask for letter 1
letter1 = input("Enter first letter: ")

# Ask for letter 2
letter2 = input("Enter second letter: ")

# Compare letter 1 and letter 2
if letter1 < letter2:
    print(f"Letter 1 {letter1} is less than letter 2 {letter2}")
elif letter1 == letter2:
    print(f"Letter 1 {letter1} is equal to letter 2 {letter2}")
else:
    print(f"Letter 1 {letter1} is greater than letter 2 {letter2}")
```
</details>

#

# Idiot Proofing

Idiot Proofing is the process in coding to make sure that if someone with a lower IQ than most is using ur program it doesn't cause fatal errors.

#

**Non Idiot Proof Code:**
```python
# Ask for ONE letter
letter = input("Enter 1 letter: ")

# Print the letter
print("You entered " + letter)

```
Now this wouldnt cause an error if you inputted more than one letter but it isn't what you are meant to input so if you handle the variable differently you can get an error.

**Idiot Proof Code:**
```python
# Ask for ONE letter
letter = input("Enter 1 letter: ")

# Print the letter
if len(letter) == 1:
    print("You entered " + letter)
else:
    print("You entered more than one letter")
```
In this case, we make sure that the user has only inputted one letter using the len function (len is short for length).

So if we did this:
```python
# Define variable
letter = "ABC"

# Print the amount of letters in the letter variable
print(len(letter))
```
We would get 3 as the output.

****
Now these are just basic examples of idiot proofing. There are many more ways but this is just so you understand the idea of idiot proofing. Ok, you can go to lesson 3 now!