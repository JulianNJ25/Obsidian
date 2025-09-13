Sometimes we need code to be run multiple times, we could call the same lines of code over and over again in our document, but if we need to print millions of numbers this can be quite the task. Loops are a great option for repetitive tasks

The **while loop** will always run the code inside it as long as the condition is TRUE
```python
while condition:
	code line1
	code line2
	code lineN
```
![[Pasted image 20250417170815.png]]Example:
```python
repeat_count = 1
while repeat_count <= 3; #while loop will repeat until our variable is less or equal to 3
	repeat_count += 1
	word = input("Give me a word: ")
	upper_word = word.upper()
	print("The word in upper-case: " + upper_word)
```

## Index-Variable Pattern
Idea: Controlling precisely how many times a loop repeats:

We can a program that repeats itself 10 times before ending
```python
index = 0            # Part 1: Declare index variable
while index < 10:  # Part 2: Compare index to condition
	print('Hi')    # Part 3: Print statement
  	index += 1     # Part 4: Math operation to add or substract from index
```

The main concept is to create a variable to control how many times the code is executed while modifying that same condition in each loop iteration

Example:
We need a program that prints a pyramid dynamically using a while loop
```python
pyramid_size = int(input("Enter pyramid size: "))
i = 1
while i < pyramid_size
	spacing = (pyramid_size - i)
	print(" " * spacing + "#" * (i*2))
	index += 1
```

## While Loop Nesting
Refers to using a loop inside a loop.

This is not always necessary, but there will be times in which a nested loop can solve a particular problem

Syntax example:
```python
i = 0
while i < 10:
	j = 0
	while j < 10:
		print("Hi")
		j += 1
	i += 1
print("Done")
	
```
This code will print Hi 10 times and will do this 10 times over as long as the 2 variables are 0

