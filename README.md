# PRG101-Lab4
### Submission Details

In this lab, you will create twelve simple scripts. Write the scripts in code spaces or close the repository and open the files in VSCode. 
Please note that you must complete the lab during class hours and show your progress to the professor to receive the marks for the lab.

### Lab Objectives
- to be able to use data type List.
- To be able to write the programs using functions.
  
## INVESTIGATION 1: LISTS

A list in Python is an ordered collection of items that can be of different types. Lists are mutable, meaning you can change their content after creation.
In this Part you will be creating lists and performing basic operations on lists using list methods and built-in functions.
Lists are used to store data elements. Usually lists contain similar kind of data, but python does not restrict you from adding values of different data types in a list.

## lab4a.py
### Creating lists and list concatenation
Lists are constructed with brackets [] and commas separating every element in the list. For example:
```Python
numbers=[1,2,3,4]
mixed_list=[1, "two", 4.5, True]
```
- Fill in the required feilds in the comment section
- Create a variable of the type list called mylist1 and save first three odd numbers (1,3,5) in it.
- Create a variable second variable of the type list and call it mylist2, save first three even numbers (0,2,4) in it.
- Create a third variable called mylist. This variable should contain all elements form mylist1 and mylist2. Remember you can use + to concatenate lists, just like we did for strings.
- Print the variable mylist.

## lab4b.py
### Using list methods to add and remove elements from a list 

- Fill in the required feilds in the comment section.
- Create 3 lists named mylist1, mylist2, and mylist (same from lab4a).
- Use the append() method and add a new element, number 7 in the variable mylist 
- Insert the element 0 at index 0.
- Pop the element from index 2.
- Print the variable mylist.
- Add another statement in the script to find the index of the element 6 and print `The element 6 is present at the index ---`

## lab4c.py
### Modifying a list and using the list in a loop
- Fill in the required feilds in the comment section.
- Create a list variable called students. Add the following names in this list: Ama, Elina, Maija, Daniel, Ibrahim.
- Next change the element at index 1 and update this element with "Maggy"
- Now use a for loop and iterate over this list and print each element on a separate line. 

## lab4d.py
### Indexing and slicing
- Fill in the required feilds in the comment section.
- Create a list variable and call it words.
- Write a while loop, in which you ask the user to enter a word or press Q to quit. Save the word in the list words or break the loop when user enters Q or q. 
- Print number of elements in the list words using `len()` function. 
- Create a new list and call it someWords.
- Assign the elements present at index 0 till 3 to the list someWords from words. Do this only if the number of elements in words is more than 3.
- Print if the list words and the list someWords are equal?
- Print the list words.
- Print the list someWords
  
## lab4e.py
### Two Dimensional Lists
A great feature of of Python data structures is that they support *nesting*. This means we can have data structures within data structures. For example: A list inside a list.
A 2D list is a list where each element is itself a list. These inner lists represent rows, and the elements within them represent columns.

```Python
matrix = [
[1, 2, 3],
[4, 5, 6],
[7, 8, 9]
]

element = matrix[1][2]  # Output: 6
```
- Fill in the required feilds in the comment section.
- Copy the above code in the file `lab4e.py`.
- Print the element `5` from this list. Specify the correct row and column.
- Print the element `2` from this list.
- Print the element `9` from this list.
- Use a for loop and print individual lists from this matrix. You need a single for loop. The output should be like this:
  ```python
  [1,2,3]
  [4,5,6]
  [7,8,9]
  ```
- Next use a nested for loop and print each individual element from the list. The output should be like this:
    ```python
  1, 2, 3
  4, 5, 6
  7, 8, 9
  ```

## INVESTIGATION 2: Functions

A function is a block of code that performs a specific task. Functions help to organize code, make it reusable, and improve readability. 
Functions help us avoid writing the same code repeatedly. If you remember, we used the len() function to determine the length of a string. Since measuring the length of a sequence like a string of list is a frequent task, it makes sense to have a function that can perform this action whenever needed.
Functions are among the most fundamental tools for reusing code in Python, and they also introduce us to the concept of program design. You should use functions when you anticipate reusing a block of code multiple times. By defining a function, you can call the same code without needing to rewrite it, which helps in creating more complex Python scripts.
Let's see how to create our own functions.

### Defining a Function

To define a function in Python, use the `def` keyword followed by the function name and parentheses `()`. Try to keep names relevant. Also be careful with names, you should not use the same name as a built-in function in Python such as `round` or `print`.
Next come a pair of parentheses with a number of arguments separated by a comma. These arguments are the inputs for your function. You'll be able to use these inputs in your function and reference them. After this you put a colon.

After colon on the next line, comes the indented block of code which is the body of the function.
Inside the body of the function, as a convention and as a good programming practice you shold start with the docstring. This is where you write a basic description of the function so that you can refer to it when you comeback to your code later or if you are working in a team, so that your team members can know what is this function about.
After the docsting you write the logic and code of your function.
Functions can also return a value or multiple values(all packed as a tuple).


#### Syntax

```python
def function_name(parameters):
    # Code block
    return value  # Optional
```
#### Example

```python
def greet(name):
    print(f"Hello, {name}!")
```

#### Explanation

- `def`: Keyword to start the function definition.
- `function_name`: The name of the function.
- `parameters`: Variables passed to the function (optional).
- `return`: Ends the function and optionally returns a value.

### Calling a Function

To execute a function, call it by its name followed by parentheses, optionally including arguments. If you forget the parenthesis (), it will simply display the statement that `greet` is a function.

#### Example
```python
greet("Alice")
Output: Hello, Alice!
```

### Function Parameters

Functions can accept parameters to make them more flexible.

#### Example

```python
def add(a, b):
    return a + b

result = add(3, 5)
print(result)
# Output: 8
```

### Default Parameters

You can define default parameter values in a function.

#### Example

```python
def greet(name="Guest"):
    print(f"Hello, {name}!")

greet()
# Output: Hello, Guest!

greet("Bob")
# Output: Hello, Bob!
```

### Return Values

Functions can return values using the `return` statement.

#### Example

```python
def multiply(a, b):
    return a * b

result = multiply(4, 5)
print(result)
# Output; 20
```

## lab4f.py 
### Simple Function

- Fill in the required feilds in the comment section.
- Write a function that  takes a list as argument and return true if any number in the list is even, the function returns false otherwise.
- Call the function with a list of 6 integer values.


## lab4g.py 
### Adding some complexity to the function  logic.

- Fill in the required feilds in the comment section.
- Write a function that  takes a list as argument and return a new list of all the even numbers from the list.
- If the passed list does not contain any even numbers, return an empty list.
- Call the function with a list of 8 integer values.

## Using the main function.
Remember you learnt in the class that we should use main function as entry point to our program.
The main() function in Python is a convention rather than a built-in function. It organizes code in a clear, structured way.
It serves as the starting point for the program. When the script is executed, the code inside the main() function runs first.
In this next example, write a function `sum` that takes two numbers as parameters and returns thier sum. You will call `sum` from `main`.

### lab4h.py 
-  Fill in the required feilds in the comment section.
-  Write a function `sum` that takes two numbers as parameters and returns thier sum
-  Write the `main` functions.
-  In the main function get two numbers from user.
-  Call the `sum` function and pass the two numbers as argument.
-  Call the main function inside the condition:
 
  ``` python
if __name__ == "__main__":
main()
```
Note that the above line checks whether the script is being run directly or being imported as a module. If it's run directly, main() is called.


## lab4i.py 
### Writing the complete calculator function using default parameters and positional parameters
Positional parameters are arguments passed to a function based on their position (order) in the function definition.
When calling the function, the first argument provided is assigned to the first parameter, the second argument to the second parameter, and so on. Default parameters are explained above. 


- Fill in the required feilds in the comment section.
- Write a function `compute` which takes three parameters; two numbers and one operation.
    - first parameter is num1
    - second parameter is num2
    - third parameters is the operation as a symbol ( +, -, *, /)
    - third parameter should have a dafult value of +

- The function perfomrs the required operation on the two numbers and returns the result. The function should receive the parameters as positional parameters.
- Write the `main` functions.
- In the main function get two numbers from user.
- In the main also ask the user to chose which operation they wnat to perform. Show the operation symbols in the prompt.
- Call the  `compute` function as follows:
    ``` python
    compute(13,45,'*')
    compute(13,45,'/')
    compute(13,45,'-')
    compute(13,45,'+')
    compute(13,45)  # since only two parameters are passed the default value of symbol should be used.
    
    ```
- Call the main function in the condiational statement as shown above in `lab4c`.

## lab4j.py 
### Writing the complete calculator function using keyword parameters
Keyword parameters (or keyword arguments) are arguments passed to a function by explicitly naming each parameter, allowing you to pass arguments out of order.
- Fill in the required feilds in the comment section.
- copy the code from lab4i.py and modify the parameters to behave as keyword parameters rather than potional parameters.
- Refer to lesson slides if you need help on how to use keyword arguments.

## lab4k.py
### Using variable number of arguments with *args
- Fill in the required feilds in the comment section.
- Write a function that returns the first letter from each provided name. It can handle a variable number of name inputs.
- The function uses `*args` to accept a variable number of name inputs.
- The function Iterate through each name and extract the first letter.
- The function collects these first letters into a list.
- Finally, the function returns the list of initials.
- Given the names "Alice", "Bob", "Charlie", and "David", the function will return the list `['A', 'B', 'C', 'D']`.

 ## lab4l.py
### Using map, filter and lambda expressions.
map() applies a function to all items in an iterable.

```Python
result = map(lambda x: x * 2, [1, 2, 3])  # Output: [2, 4, 6]
```

filter() selects items from an iterable based on a function that returns True or False.

```Python
result = filter(lambda x: x > 2, [1, 2, 3, 4])  # Output: [3, 4]
```

lambda creates small, anonymous functions for quick, on-the-fly use.

```Python
square = lambda x: x ** 2  # Usage: square(3) -> 9
```
- Create a variable list named numbers containing numbers from 2 to 10.
- Sqaure all elements of this list using map and lambda function.
- Print variable numbers.
- Make a new variable named divisibleby2.
- Filters out all numbers from numbers list that are divisible by 2 using filter and lambda, and save them in this variable.
- Print variable divisibleby2.

## Lab 3 Sign-Off
- Submit the screenshots of each individual script, the screenshot must show your scripts and command line interface and output.
- The screenshot must also show your username on github codespaces.
- Submit individual screenshots of the following scripts on blackboard. If the screenshots do not correctly show the information mentioned above, you will get zero marks for the lab.
    - lab4a.py
    - lab4b.py
    - lab4c.py
    - lab4d.py
    - lab4e.py
    - lab4f.py
    - lab4g.py
    - lab4h.py
    - lab4i.py
    - lab4j.py
    - lab4k.py
    - lab4l.py


