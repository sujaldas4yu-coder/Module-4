# 🔤 Dictionary-Python Program to Sort a Dictionary by Keys and Values

This Python program demonstrates how to sort a dictionary:
- Alphabetically by keys
- Alphabetically by values

---

## 🎯 Aim

To write a Python program that sorts a dictionary's:
- Keys in alphabetical order
- Values in alphabetical order

---

## 🧠 Algorithm

1. **Start the program.**
2. **Define** a dictionary with key-value pairs.
3. **Sort by Keys**:
   - Use `sorted(dictionary.items())`
   - Convert the result to a dictionary using `dict()`
4. **Sort by Values**:
   - Use `sorted(dictionary.items(), key=lambda item: item[1])`
   - Convert the result to a dictionary using `dict()`
5. **Display** the original and sorted dictionaries.
6. **End the program.**

---

## 🧪Program
```
# Sort a Dictionary by Keys and Values

dictionary = {
    'banana': 'yellow',
    'apple': 'red',
    'grape': 'purple',
    'orange': 'orange'
}

# Sort by keys
sorted_keys = dict(sorted(dictionary.items()))

# Sort by values
sorted_values = dict(sorted(dictionary.items(), key=lambda item: item[1]))

print("Original Dictionary:")
print(dictionary)

print("\nDictionary Sorted by Keys:")
print(sorted_keys)

print("\nDictionary Sorted by Values:")
print(sorted_values)
```

## Sample Output:
```
Original Dictionary:
{'banana': 'yellow', 'apple': 'red', 'grape': 'purple', 'orange': 'orange'}

Dictionary Sorted by Keys:
{'apple': 'red', 'banana': 'yellow', 'grape': 'purple', 'orange': 'orange'}

Dictionary Sorted by Values:
{'orange': 'orange', 'grape': 'purple', 'apple': 'red', 'banana': 'yellow'}
```

