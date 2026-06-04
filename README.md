# Regex in Python: Filter Words Without the Letter 'e'

## 🎯 Aim
To write a Python program that filters out and returns all elements from a list **that do not contain the letter `'e'`**, using **regular expressions (regex)**.

## 🧠 Algorithm
1. Import the `re` module.
2. Initialize an empty list `l1` to store results.
3. Define a list of words:  
   `items = ['goal', 'new', 'user', 'sit', 'eat', 'dinner']`
4. Iterate through each word in the list:
   - Use `re.search(r"e", i)` to check if the word contains `'e'`.
   - If **not**, append the word to `l1`.
5. Print the final filtered list.

## 🧾 Program
```
import re

l1 = []

items = ['goal', 'new', 'user', 'sit', 'eat', 'dinner']

for i in items:
    if not re.search(r"e", i):
        l1.append(i)

print(l1)
```
## Output

<img width="338" height="83" alt="image" src="https://github.com/user-attachments/assets/88cc9cc8-eac2-4eac-a217-1038f5f94581" />

## Result
the code ids executed

# Module-3
# 🧹 Strings-Remove Nth Index Character from a String

## 🎯 Aim
To write a Python program that accepts a string and removes the character at a specified index.

## 🧠 Algorithm
1. Define a function named `remove` that takes the input string as an argument.
2. Read the index `n` from the user input.
3. Initialize an empty string `a` to store the new string.
4. Iterate over each index of the string using a `for` loop.
5. Check if the current index `i` is not equal to `n`.
6. If `i != n`, append the character at index `i` to string `a`.
7. After the loop, return the modified string `a`.
8. Print the final result.

## 💻 Program
```
def remove(s):
    n = int(input("Enter the index to remove: "))
    a = ""

    for i in range(len(s)):
        if i != n:
            a += s[i]

    return a


string = input("Enter a string: ")
result = remove(string)
print("Modified string:", result)
```
## Output

<img width="348" height="110" alt="image" src="https://github.com/user-attachments/assets/752c348d-0876-44fa-a5c8-a3e4bb14ee54" />


## Result
the code is executed


# Strings-Palindrome Check in Python (Without Built-in Functions)

## 🎯 Aim
To write a Python program to check whether the string `"google"` is a **palindrome** or not, without using built-in palindrome checking functions.

## 🧠 Algorithm
1. Assign the string `"google"` to a variable.
2. Reverse the string manually using slicing (`[::-1]`).
3. Compare the original string with the reversed string.
   - If they are equal, print that the string is a palindrome.
   - Otherwise, print that it is not a palindrome.
4. Execute the program.

## 🧾 Program
```
def is_palindrome(s):
    rev = ""
    for ch in s:
        rev = ch + rev   # build reverse manually

    if s == rev:
        return "Palindrome"
    else:
        return "Not a Palindrome"
word = input("Enter a string: ")
print(is_palindrome(word))
```

## Output

<img width="533" height="197" alt="image" src="https://github.com/user-attachments/assets/d514bae1-ebe0-4acd-be88-41a00b96b89a" />


## Result
the code is executed




