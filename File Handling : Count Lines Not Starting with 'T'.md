# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program
```
count = 0

with open("story.txt", "r") as file:
    for line in file:
        if line and line[0] != 'T':
            count += 1

print("Number of lines not starting with 'T':", count)
```

## Output
```
If "story.txt" contains:

This is the first line
Apple is a fruit
Today is sunny
Banana is yellow

Number of lines not starting with 'T': 2
```
