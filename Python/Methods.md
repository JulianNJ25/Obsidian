**Methods** are operations specific to a type of value, meaning strings, ints, floats, and more have their own unique methods

What we get from methods is called **return value** 

Performing a method on a value is known as **calling the method**, this process is done by placing a **dot ****.** between the value  and the method name

Some other methods can also take extra information either optionally or not. This information is known as **arguments** 

## String Methods
**.format()**
	Formats strings with placeholders inside of curly braces `{ }` inside them. The placeholders will be filled with the arguments passed inside `.format()`. Note that **f-string** might be faster and cleaner to use
```python
		name = "Alex"
		age = 21
		print("My name is {} and I am {} years old.".format(name, age))
```
	We can also format by indexing our arguments
```python
		print("My name is {0} and I am {1}. {0} is a nice name.".format(name, age))
```
	We can also format numbers to show an specific amount of decimal numbers
```python
		pi = 3.1416
		print("Value of pi is {:.1f}".format(pi))
```

**.upper()**
	converts a string to uppercase
		`"hello".upper()` -> "HELLO"

**.strip()**
	Removes empty spaces in a string or the selected characters in the argument
		`"   hello    ".strip()`-> "hello"
		`"hello".strip(el)` -> " ho"

**.count()**
	Returns the number of occurrences of the argument's chars in the used string
		`'abc'.count('a')`
			returns -> 1
		`'abc'.count('q')`
			returns -> 0
	Occurrences might overlap, in which case only the first occurrence is taken in account
		`'ababa'.count('aba')`
			returns -> 1

**.isupper()**
	Determines whether a character is uppercase or not, *returns boolean*
```python
>>> 'q'.isupper()
False
>>> 'Q'.isupper()
True
```
## Number Methods
.bit_length()
	Returns the amount of memory used by an integer, to parentheses the int number is a must
		`(5).bit_length()`
		returns -> 3