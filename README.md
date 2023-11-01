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

#### split() : 

default : space , new line & carriage return

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



### Tuple : immutable ordered sequences of elements.

    - often used to store related pieces of information.
    - can be indexed and sliced like a list.
    - example involving latitude and longitude:
           location = (13.4125, 103.866667)
           print("Latitude:", location[0])
           print("Longitude:", location[1])
           
   #### Tuple Unpacking
   Tuples can also be used to assign multiple variables in a compact way.

     dimensions = 52, 40, 100
     length, width, height = dimensions
     print("The dimensions are {} x {} x {}".format(length, width, height))
         
   ##### The parentheses are optional when defining tuples, and programmers frequently omit them if parentheses don't clarify the code. 
         
   In the second line, three variables are assigned from the content of the tuple dimensions. This is called tuple unpacking. You can use tuple unpacking to assign the 
   information from a tuple into multiple variables without having to access them one by one and make multiple assignment statements.

### Sets : mutable unordered collections of unique elements.

   - One application of a set is to quickly remove duplicates from a list.
   - can modify the elements in a set with methods like add and pop.
   - can't index and slice elements like a list; there is no sequence of positions to index with!
   - only contains unique elements.
   - defined with curly braces, {}
   - set_example = {element1, element2, element3}
   - empty set of curly braces like this: a = {}


         numbers = [1, 2, 6, 3, 1, 1, 6]
         unique_nums = set(numbers)
         print(unique_nums)

        This would output:  {1, 2, 3, 6}

   - Used Operations :
        - add
        - in
        - pop : random element is poped since set is an unordered container
    
### Dictionaries & Identity Operators

   #### Dictionary: mutable data type that stores mappings of unique keys to values.

            - {key1:value1, key2:value2, key3:value3, key4:value4, ...}
            - Dictionaries are mutable, but their keys need to be any immutable type, like strings, integers, or tuples.
            - It's not even necessary for every key in a dictionary to have the same type!
            - keys are used to index values, they must be unique and immutable.

       
   - Used Operations :
        - in
        - get : looks up values in a dictionary, but unlike square brackets*,* get returns None (or a default value of your choice) if the key isn't found.
 
  
  ####  Identity Operators
    
            - is	: evaluates if both sides have the same identity
            - is not: evaluates if both sides have different identities

  #### Practice : ==  vs. is

         a = [1, 2, 3]
         b = a
         c = [1, 2, 3]
         
         print(a == b)  //True
         print(a is b)  //True
         print(a == c)  //True
         print(a is c)  //False



<img width="1246" alt="Screenshot 2023-10-26 at 1 35 16 AM" src="https://github.com/AditiRai17/AWS-AI-ML-/assets/91966396/a9329102-84ad-41db-8c40-d8a4eae26efa">


## Control Flow

  - Conditional Statements
  - Boolean Expression
  - For and While Loops
  - Break and Continue
  - Zip and Enumerate
  - List Comprehensions

  ### Conditional Statements : if , elif , else
  
*  #### Indentation : The Python Style Guide (PEP 8) recommends using 4 spaces to indent, rather than using a tab.

  Here are most of the built-in objects that are considered False in Python:

     - constants defined to be false: None and False
     - zero of any numeric type: 0, 0.0, 0j, Decimal(0), Fraction(0, 1)
     - empty sequences and collections: '"", (), [], {}, set(), range(0)


 ### Loops : do something repeatedly, over an iterable.

   - An iterable is an object that can return one of its elements at a time. 
   - This can include sequence types, such as strings, lists, and tuples, as well as non-sequence types, such as dictionaries and files.
   - range() is a built-in function used to create an iterable sequence of numbers.
     
   ##### range() 

       range(start=0, stop, step=1)
       
       The range() function takes three integer arguments, the first and third of which are optional:
       
       - The 'start' argument is the first number of the sequence. If unspecified, 'start' defaults to 0.
       - The 'stop' argument is 1 more than the last number of the sequence. This argument must be specified.
       - The 'step' argument is the difference between each number in the sequence. If unspecified, 'step' defaults to 1.
       
       Notes on using range():
       
       If you specify one integer inside the parentheses withrange(), it's used as the value for 'stop,' and the defaults are used for the other two.
           e.g. - range(4) returns 0, 1, 2, 3
       If you specify two integers inside the parentheses withrange(), they're used for 'start' and 'stop,' and the default is used for 'step.'
           e.g. - range(2, 6) returns 2, 3, 4, 5
       Or you can specify all three integers for 'start', 'stop', and 'step.'
           e.g. - range(1, 10, 2) returns 1, 3, 5, 7, 9

   #### For loop 

        

        

      



