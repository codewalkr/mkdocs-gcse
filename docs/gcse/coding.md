# Coding Practice

1. The Total & Average Pattern

This is the "bread and butter" of computational thinking: iterating through a set of data to calculate a result.

```python
scores = [45, 87, 32, 91, 55]
total = 0

for s in scores:
    total = total + s

average = total / len(scores)
print("Average score is:", average)
```

2. The Linear Search

You will almost certainly be asked to write or complete a search algorithm.

```python
items = ["Apple", "Banana", "Cherry"]
target = input("Search for: ")
found = False

for i in range(len(items)):
    if items[i] == target:
        found = True
        print("Found at index", i)

if found == False:
    print("Not in list")
```


3. Input Validation (The While Loop)

Exams love "defensive programming." This ensures the user enters a value within a specific range.

```python
age = int(input("Enter age (11-18): "))

while age < 11 or age > 18:
    print("Invalid age!")
    age = int(input("Enter age (11-18): "))

print("Age accepted")
```

4. Finding the Maximum Value

A classic "Computational Thinking" task: comparing values to find the highest.

```python
numbers = [12, 45, 2, 88, 34]
max_val = numbers[0]

for x in numbers:
    if x > max_val:
        max_val = x

print("Highest number is:", max_val)
```

