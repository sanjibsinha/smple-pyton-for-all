**2. Loops (`for` and `while`)**

Loops allow you to repeat a block of code multiple times.

*   **`for` loop:** Used when you know how many times you want to repeat the code. Often used to iterate through *iterable* objects (like lists, strings, etc.).

```python
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:  # Iterating through a list
    print(fruit)

for i in range(5):  # range(5) generates numbers from 0 to 4. Useful for repeating a specific number of times
    print(i)

for i in range(2, 7, 2): # Start at 2, stop before 7, increment by 2
    print(i) # Output: 2, 4, 6

# Iterating through a string
message = "Hello"
for char in message:
    print(char)

```

*   **`while` loop:** Used when you want to repeat code *until* a certain condition becomes `False`.  Be careful with `while` loops – if the condition never becomes `False`, you'll have an *infinite loop*!

```python
count = 0
while count < 5:
    print(count)
    count += 1  # Important: This increments the counter, preventing an infinite loop

# Example with user input:
user_input = ""
while user_input != "quit":
    user_input = input("Enter something (or 'quit' to exit): ")
    if user_input != "quit":
        print("You entered:", user_input)
```

**3. `break`, `continue`, and `pass`**

These are special statements that affect loop behavior.

*   `break`:  Immediately exits the loop.

```python
for i in range(10):
    if i == 5:
        break  # Exit the loop when i is 5
    print(i) # Output: 0, 1, 2, 3, 4
```

*   `continue`: Skips the rest of the current iteration and goes to the next one.

```python
for i in range(10):
    if i % 2 == 0:  # If i is even
        continue  # Skip to the next iteration
    print(i) # Output: 1, 3, 5, 7, 9
```

*   `pass`: Does nothing.  It's a placeholder when you need a statement syntactically, but you don't want to execute any code.  Commonly used in functions or classes that you'll define later.

```python
for i in range(5):
    if i == 2:
        pass  # Do nothing when i is 2
    else:
        print(i) # Output: 0, 1, 3, 4

def my_function():
    pass # We'll add code here later

```

