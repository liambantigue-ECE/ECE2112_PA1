# ECE2112_PA1
## EXPERIMENT 1: INTRODUCTION TO PYTHON PROGRAMMING
Liam S. Bantigue | 2ECE-A

OBJECTIVES:
At the end of this laboratory activity, the student should be able to:
1. use basic Python functions, operators, and string operations;
2. manipulate strings using indexing, slicing, and built-in string methods;
3. apply sequence unpacking to manipulate the elements of a list; and
4. construct simple Python functions that return a specified result.

# A. Word Rotation Problem
The word rotation problem instructs us to (1) create a function named "rotate_word" with the parameter named "text" that accepts a non-empty string, (2) puts the first letter at the end while keeping the rest at their original position, (3) and preserves the capitalization.

## A1. First, create a python function:
Syntax: **def function_name(parameter):**

1. **def** is the keyword to use to define a function.
2. **function_name** is as the word suggests, it is the name of the function.
3. **parameter**, is what "value" the function accepts, in our case a string.
4. and lastly, it is ended with a colon "**:**"

## A2. Second, identify the number of characters
To identify the number of characters our string has, use the len function.

Syntax: **variable = len(parameter)**

we store the gotten no. of characters to variable n so that we can just plug n in our next step

## A3. Last is python slicing
Syntax: **parameter[index of starting char:no. of char:no. of increments]**

1. First, we  start with index 1 = second letter
2. Second, use n to get the no. of characters our text has
3. Third, increment by 1 to get all characters one by one until n.
4. Lastly, we add the first character at the end by using the operator "+" and parameter[0].

# B. Username Builder Problem
The username builder problem instructs us to (1) create a function that accepts two string namely first_name and last_name, (2) change the capitalization to lowercase then (3) add them together with a period in the middle.

## B1. First, create the function with required parameters
Syntax: **def make_username(first_name, last_name):**

## B2. Turn capitalizations into lowercase and remove spaces
We can use methods such as .upper() and .replace() then store them into a new variable

Syntax: **variable = parameter.upper().replace(old, new)**

ex. first = first_name.lower().replace(" ", "")

## B3. Add the two strings with a period in between
We can simply use the operator "+" with "." in the middle to add a period when connecting the two strings together 

ex. first + "." + last

(**note**) last is the variable used to store the new processed string of parameter last_name


# C. Bookend Swap Problem
The bookend swap problem instructs us to (1) create a function name swap_bookend() with parameter named "items" that accepts a list containing at least 2 elements, (2) unpack the list into 3 variables, and (3) swap the first and last variables while retaining the middle variable.

## C1. Create function
Syntax: **def swap_bookend(items):**

## C2. First, Middle, Last Variables
Remember that when we create multiple elements we separate them with a comma ",". We can also use this but modify it a little bit to our advantage.

Syntax: parameter = first, *middle, last 

Notice the asterisk on the variable middle, this means that whatever is left in between the variable first and last, is considered the middle variable. This method is also known as *Extended Unpacking*

## C3. Swapping
Lastly, we can once again use the operator "+" to connect all of them together

Syntax: [last] + middle + [first]
