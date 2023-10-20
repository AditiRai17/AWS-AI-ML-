# AWS-AI-ML-

## Data Types and Operators

### Arithmetic operators

- Addition +
- Subtraction -
- Multiplication *
- Division /
- Mod (the remainder after dividing) %
- Exponentiation (note that ^ does not do this operation, as you might have seen in other languages) **
- Caret : bitwise XOR ^
- Divides and rounds down to the nearest integer //

The usual order of mathematical operations holds in Python, often referred to as 
#### PEMDAS: Parentheses, Exponents, Multiplication/Division, Addition/Subtraction.

### Assignment Operators 

https://www.programiz.com/python-programming/operators

#### In general, there are two types of errors to look out for
 - Exceptions : occurs when the code is running,
 - Syntax : detected when Python checks the code before it runs it.


##### The bool data type holds one of the values True or False, which are often encoded as 1 or 0, respectively.

### String Method
#### format() 

https://docs.python.org/3.6/library/string.html#format-string-syntax

#### split()

A helpful string method when working with strings is the .split method. This function or method returns a data container called a list that contains the words from the input string. We will be introducing you to the concept of lists in the next video.

The split method has two additional arguments (sep and maxsplit). The sep argument stands for "separator". It can be used to identify how the string should be split up (e.g., whitespace characters like space, tab, return, newline; specific punctuation (e.g., comma, dashes)). If the sep argument is not provided, the default separator is whitespace.

True to its name, the maxsplit argument provides the maximum number of splits. The argument gives maxsplit + 1 number of elements in the new list, with the remaining string being returned as the last element in the list. You can read more about these methods in the Python documentation too.

https://docs.python.org/3/library/stdtypes.html#string-methods


## Data Structures in Python
  - Types of Data Structures: Lists, Tuples, Sets, Dictionaries, Compound Data Structures
  - Operators: Membership, Identity
  - Built-In Functions and Methods


### List : data type for mutable ordered sequence of elements
       - create a list with square brackets. Lists can contain any mix and match of the data types you have seen so far.
       - e.g. list_of_random_things = [1, 3.4, 'a string', True]

  #### Slicing : lower index is inclusive and the upper index is exclusive.
  #### Membership Operators
         - Keyword	Operator
         - in	: evaluates if an element exists within our list
         - not in	: evaluates if an element does not exist within our list

  #### Mutability & Order
       -> String is immutable & ordered sequence of character (No changes can be made)
       -> List is mutable (changes can be made)


       - "Order" is about whether the position of an element in the object can be used to access the element.
       - Both strings and lists are ordered.
       - We can use the order to access parts of a list and string.

  #### Useful Functions for Lists 
  
- len() returns how many elements are in a list.
- max() returns the greatest element of the list. How the greatest element is determined depends on what type of objects are in the list. The maximum element in a list of numbers is the largest number. The maximum element in a list of strings is the element that would occur last if the list were sorted alphabetically. This works because the the max() function is defined in terms of the greater than comparison operator. The max() function is undefined for lists that contain elements from different, incomparable types.
- min() returns the smallest element in a list. min is the opposite of max, which returns the largest element in a list.
- sorted() returns a copy of a list in order from smallest to largest, leaving the list unchanged. Note again that for string objects, sorted smallest to largest means sorting in alphabetical order.
- join method : takes a list of strings as an argument, and returns a string consisting of the list elements joined by a separator string.
- append method : adds an element to the end of a list.


------------------------------

A data type is just a type that classifies data. This can include primitive (basic) data types like integers, booleans, and strings, as well as data structures, such as lists.
Data structures are containers that organize and group data types together in different ways. For example, some of the elements that a list can contain are integers, strings, and even other lists!
