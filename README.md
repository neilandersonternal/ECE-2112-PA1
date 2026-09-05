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

The main function for this problem is:

● ```return``` - statement is used inside a function to send a value or result back to the code that called it.

In this case I input "text[1] + text[0]" so that the output will start at the 
second letter while it will end with the supposedly first letter.

```python
def rotate_word(text):
    return text [1:] + text[0]
```


# **B. Username Builder Problem**

**Objective:**
Create a function named make username() that accepts two strings: first name and last name. The
function must: 
1. convert all letters to lowercase;
2. remove all spaces from the first name;
3. remove all spaces from the last name; and
4. join the processed first and last names using one period (.).

The following are the function that are mainly used for this problem: 

● ```lower()``` - method converts all uppercase characters in a string to lowercase.

This function is used for the first objective, which is to convert all letters to lowercase.

● ```replace()``` - This function replaces occurences of a specified substring within a string to a new substring

This function is used to remove the spaces in the substrings.

```python
def make_username(first_name, last_name):
    username_first = first_name.lower().replace(" ", "")
    username_last = last_name.lower().replace(" ", "")
    return username_first + "." + username_last
    
```

# **C. Bookends Swap Problem**


**Objective:**
Create a function named swap bookends() that accepts a list containing at least two elements. Unpack
the list into three variables:
• first – the first element;
• middle – a list containing everything between the first and last elements; and
• last – the last element.
Using these variables, return a new list in which the first and last elements have exchanged positions.
The elements in middle must remain in their original order. Do not modify the input list.

The main function that is used for this problem is:

● ```return``` - statement is used inside a function to send a value or result back to the code that called it.

This problem is almost the same with first problem, but in this case, the two ends
of the elements (first element, last element) should swap while maintaining the element/s between them.
So, I used the return function to modify the sequence by putting the "[last]" element on first, and 
"[first]" element on last.


```python
def swap_bookends(items):
    first, *middle, last = items
    return [last] + middle + [first]
```



That's all for my first assignment about base computing with python. Thank you!!

**README file version history:**

August 26, 2026: Initial README output uploaded.

August 30, 2026: Revied format README was uploaded.

September 5, 2026:  python code example was enhanced.

















  



