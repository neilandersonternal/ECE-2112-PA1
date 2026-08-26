## **ECE-2112-PA-1**

**This is made by Neil Anderson D. Ternal from 2ECE-D**

This is mainly for the content of the repository that I've submitted which covers the three Python problems from our assignment from the course
ECE 2112(Advanced Computer Programming). In which includes Base Computing using Python as a language.

So, for the first problem.



# **A. WORD ROTATION PROBLEM**

**Objective:**
Create a function named rotate word() that accepts a non-empty string. Move the first character
of the string to the end while keeping all remaining characters in their original order. Preserve the
capitalization of every character.

Example: 
print (rotate_word("ECED")) >> CEDE (the E at the first, ends up in the last)


So, for the first thing that I did was to define the function with the name of "rotate_word". 
After that, I used the return function in order to alter the value for the output. With the **return** function,
I input "text[1] + text[0]" so that the output will start at the second letter while it will end with the
supposedly first letter.

```
def rotate_word(text):
    return text [1:] + text[0]
```
With that, the I've solved the first problem.




# **B. Username Builder Problem**

**Objective:**
Create a function named make username() that accepts two strings: first name and last name. The
function must: 
1. convert all letters to lowercase;
2. remove all spaces from the first name;
3. remove all spaces from the last name; and
4. join the processed first and last names using one period (.).


First, create a user-defined function with "def", and as for the instruction that was indicated from our assignment,
the name of the function should be "make_username". After that, to set the first name into lowercase, I added another name, for the
first name itself, after that I used the **lower()** function in order to convert all uppercase characters in a string into lowercase.
With the same method, I also made the last name into lowercase to fully accomplish the main goal, which is converting names into lowercase. 
For the final touch, I used the function **return**, to input "." between the first name and last name.

```
def make_username(first_name, last_name):
    username_first = first_name.lower().replace(" ", "")
    username_last = last_name.lower().replace(" ", "")
    return username_first + "." + username_last
    
```
And with that, I managed to solve the second problem.

# **C. Bookends Swap Problem**


**Objective:**
Create a function named swap bookends() that accepts a list containing at least two elements. Unpack
the list into three variables:
• first – the first element;
• middle – a list containing everything between the first and last elements; and
• last – the last element.
Using these variables, return a new list in which the first and last elements have exchanged positions.
The elements in middle must remain in their original order. Do not modify the input list.

For this problem, this is easier than the second problem since this problem is like the first problem. The only difference
that will make for this problem is that the first and last elements will only swap position while maintaining the second
element in their own position. So for this, I just created a defined function again with the name "swap_bookends". 
So after that, I indicated the format which is "first, *middle, last = items ". And for the main and final touch,
I put a **return** function with putting first the "last" element inside the [] and putting "first" element as the last.

so for the actual code, this is:
```
def swap_bookends(items):
    first, *middle, last = items
    return [last] + middle + [first]
```



That's all for my first assignment about base computing with python. Thank you!!


















  



