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

