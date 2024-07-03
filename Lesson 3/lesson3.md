# Welcome to lesson 3
In this lesson we will learn about lists, saving data to file, and reading data from files and maybe how to use modules!

**Part 1**

Lists

 How to make a list
```py
list_one = ["one", "two", "apple", "banana"]

print(list_one)
```
This would print ["one", "two", "apple", "banana"]
Which all things considered, is pretty ugly, so we can make it better like this

```py
list = ["one", "two", "apple", "banana"]

for i in list:
    print(i)
```
This would print:
```
one

two

apple

banana
```

**How to add things to the list**

To add an object to a list, we use the append method:
```py
# Make a list of fruit
fruit = ["apple", "banana"]

# Print current list
print("List before append: ", fruit)

# Would print: List before append:  ['apple', 'banana']

# Add "orange" to the list
fruit.append("orange")

# Print new list
print("List after append: ", fruit)

# Would print: List after append:  ['apple', 'banana', 'orange']

# Now remove "banana" from the list
fruit.remove("banana")

# Print new list
print("List after remove: ", fruit)

# Would print: List after remove:  ['apple', 'orange']
```


# Part 2 - Saving Data to File

Saving data to a file is simple in python, here is a quick example

```py
# Open a file in write mode
with open("file.txt", "w") as file:
    # Write some text to the file
    file.write("Hello, World!")
```

This would create a file named "file.txt" with the text "Hello, World!" in it.

Now here is some more advanced stuff

```py
# Make a list of fruit
fruits = ["apple", "banana", "orange"]

# Ask user for a new fruit
new_fruit = input("Enter a new fruit: ")

# Add the new fruit to the list
fruits.append(new_fruit)

# Open a file in write mode
with open("fruit.txt", "w") as file:
    # Write all the fruit into the file on their own line
    for fruit in fruits:
        file.write(fruit + "\n")
    print("Saved All fruit to file fruit.txt")
    for fruit in fruits:
        print(fruit)
```
This script has a default list of fruits, then asks the user for a new one, then saves all of the fruits to a file named fruit.txt


Now its your turn.

Make a script that has a default list of countries, then asks the user for a new one, then saves all of the countries to a file named countries.txt (Write all of this in main.py)

**__DO NOT PASTE FROM CODE ABOVE__**

Write it yourself.


#
# Part 3. Reading data from files

To get the full contents from a file, we use the read method

```py
# Open a file in read mode
with open("fruit.txt", "r") as file:
    # Read all the text from the file
    text = file.read()
    print(text)
```

To get a certain line from a file, we use the readline method

```py
# Open a file in read mode
with open("fruit.txt", "r") as file:
    # Read the first line
    line = file.readline()
    print(line)
```

To get the amount of lines in a file, we use the len method

```py
# Open a file in read mode
with open("fruit.txt", "r") as file:
    # Read all the lines
    lines = file.readlines()
    print(len(lines))
```

Now in main2.py, Write a script that gets file information from data.txt

The data should be this:
```
Lines: int()
First Line: str()
Last Line: str()

Full File: str()
```

# Part 4. Modules
Modules are like addons to python, they can be used to make your life easier.

example, using the requests module, we can send a request to a website and get the response
```py
# Import the requests library
import requests

# Get a response from example.com
response = requests.get("https://example.com")

# Print the response
print(response.text)
```

Now, some modules don't come pre-installed with python, so we will need to use the `pip` command to install them

Example:
```
pip install requests
```
