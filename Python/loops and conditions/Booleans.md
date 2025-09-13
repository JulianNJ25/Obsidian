Booleans is another data type it only has two possible values `True` or `False` and as with the other variables, we don't need do specify its type when declaring them
```python
theSkyisBlue = true
theSkyisRed = false
```

We can work with boolean values without the need of declaring them as well, such as with math operations thanks to **boolean expressions**

**Boolean expressions** are the result of boolean operations rather than a numeric value (even though we can understand the result in 1 or 0)
```python
enough_monery = 1000 > 10           #This will be True
do_the_names_match = Ryan  == Nayr  #This will be False
```

**Boolean operation** include, but are not limited to:

| Operators | Meaning               |
| --------- | --------------------- |
| <         | less than             |
| >         | greater than          |
| <=        | less or equal than    |
| >=        | greater or equal than |
| ==        | equal                 |
| !=        | not equal             |
| in        | is part-of            |

Boolean operations can be done to Integers, Floats, and Strings. For example, what if we canted to write a program that checks if a user can afford a 20% down-payment to purchase a house. We can write an **if-statement**:
```python
home_cost = int(input('How much does the home cost: '))
available_funds = int(input('What are your available funds: '))
down_payment = home_cost * 0.2

if available_funds >= down_payment
	print('You can afford a down payment!')
```

Booleans are used in a wide range of options thanks to Control Flow, introduction code is read from top to bottom, however we can run our code in a wide variety, and code has no rule to being linear. Different ways we can control our code is through:
- [[If-Statements]]
- [[While Loops]]
- [[For Loops]]

### Boolean Operators
#### 'or' Operator
The or operator returns **true** as long as **one of the conditions** is true. The only way of making 'or' return false is if the two conditions are false
```python
>>> True or True
True
>>> True or False
True
>>> False or True
True
>>> False or False
false
```

#### 'and' Operator
The and operator returns **true** if both of its operands are True, if either one of the operands are false, it will return false
```python
>>> True or True
True
>>> True or False
false
>>> False or True
false
>>> False or False
false
```
#### 'not' Operator
Unlike *and* and *or*, the not operator only takes **one operand**
```python
>>> not True
False
>>> not False
True
```
#### Precedence
The precedence of **and** is **higher** than **or**, here is an example of why this is important:
```python
>>> True or True and False
True
```
Python interprets this expression as:
```python
>>> True or (True and False)
True
```
If we use parentheses to change the logic of this comparison we will get a completely different result
```python
>>> (True or True) and False
False
```

The precedence of **not** is **higher** than *or* and *and*

### Operators in Strings
Operators can also tells us the alphabetical order or strings and whether or not they have uppercase characters

- One string is less than another if it comes first in alphabetical order
Example:
	>>> brave < cave
	true
	>>>cave < cavern 
	true
	>>>orange < apple
	false

- Due to how uppercase characters are stored in memory, uppercase characters come before lowercase ones
Example:
	>>> apple < Banana
	false

- One relational operator that works on string and not in numbers is the **in** operand
Example:
	>>> 'ppl' in 'people'
	true
	>>> 'ale' in 'apple'
	false