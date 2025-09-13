**For loops** are useful when we know exactly for how long we want to repeat our loop meaning they are a *definite loop*, as the number of iterations is predetermined

The structure of a For Loop is the **for** keyword that initiates the loop, the **loop variable**, this variable can have any name an will represent each single element in the loop. In the case of a String it will represent each letter of the String.

Its a good practice to name the loop variable with a contextual name for better readability
Syntax example:
```python
before code
for index in range(0, 4):
	inner code
after code
```

This code will repeat itself until (in this case) `index` gets to the value of 3. The loop will end when the variables reaches 1 less than the second number specified in `range`

One execution of the loop is referred to as an *iteration*. This iteration will repeat N number of times according to the length of the sequence. Meaning if we are iterating
through a String we can know how many loops will occur with the `len()` method
```python
>>> len('olive')
5 #if we used a for loop in olive string, the loop will run 5 times
```

![[Pasted image 20250418124540.png]]

### Range for loops
Python **range** function generates ranges of integers that help us control for loops. So instead of parsing through all the characters in a string we can loop through integers
"Practical" example:
```python
>>> for num in range(5):
		print(num)
0
1
2
3
4
--------------------------------------------------------------------------
```
```python
print("before")
for i in range(1, 5):
	print("Hi")
	print('i variable is: ' + str(i))
print('after')
```
```
before
hi
i variable is: 1
hi
i variable is: 2
hi
i variable is: 3
hi
i variable is: 4
after
```

By default python counts one by one, but we can include a third argument to tell python different **step sizes**
```python
>>> for num in range(0, 10, 2):
		print(num)
0
2
4
6
8

-----------------------------------------------------------

>>> for num in range(0, 10, 3)
		print(num)
0
3
6
9
```

We can also **count backwards**
```python
>>> for num in range(6, 2, -1)
		print(num)
6
5
4
3

----------------------------------------------------------------

>>> for num in range(6, -1, -1): #we use -1 as the second argument to count ot 0
		print(num)
6
5
4
3
2
1
0
```

==Note: to quickly look at the numbers inside a range we can use the following piece of code==
```python
>>> list(range(3, 7))
>>> print(list)

[3, 4, 5 ,6]
```
