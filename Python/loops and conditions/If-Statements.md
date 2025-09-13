We can create code that selectively or conditionally run according to a condition. A fundamental part of computer programming

The general form of **if-statements** is the following:
```python
code A
if condition:
	code B
code C
```

this can be translated to:
```
if "conditon" is true
	run B
if is not, run C
```

Example -> program that tells a user if you earned more money than you spent
```python
earned = int(input('How much money did you earn? '))
spent = int(input('How much money did you spend? '))
if earned > spent:
	print("You earned more than you spent")
if earned == spent:
	print("You are even with money")
if earned < spent;
	print("You should spend less")
```

**And / Or**
Life often has complex decision than are more difficult to solve with simple "if" checks. Thats why we can use boolean logic into our code with the keywords **and** & **or**

**and** -> if both values are TRUE then TRUE -> ELSE = FALSE
**or** -> if either side or both are TRUE then TRUE -> if both sides are FALSE then FALSE
![[Pasted image 20250417163849.png]]

Example -> program that checks if you height is allowed in a roller coaster ride
```python
height = int(intpu("Height in inches: "))
if height >= 40 and height <= 70
	print("you may ride")
if height < 40 or height > 70
	print("You may not ride")
```

## If-Else

Constantly checking if statements can get redundant, we can infer that if our option was not valid the FALSE condition has been met, instead of coding another "if" check, we can simply run our remaining code using the `else` keyword
```python
earned = int(input("How much you earned: "))
spent = int(input("How much you spent: "))
if earned >= spent
	print("You did not overspend")
else
	print("You did overspend")
```
![[Pasted image 20250417165312.png]]
## Elif
Sometimes we do need to have multiple choices, Elif is a way to add multiple if statements in a block of code
```python
if conditionA:
	print('something')
elif conditionB:
	print('somethingB')
else:
	print('SomethingC')
	
```
![[Pasted image 20250417170029.png]]