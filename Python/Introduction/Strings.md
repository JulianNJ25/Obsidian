[[Variables]] that allow us to store series of letters to form words.

Can be enclosed inside double and single quotes
*'This is a string'* *"This is also a string"*

We declare strings by creating the variable name and assigning  its value
```python
character_1 = 'Jhon'
```

String variables can also be put together by [[Concatenation]]
```python
character_1 = "Jhon"
character_2 = "Pork"

Print(character_1 + character_2)
Print(character_1, character_2)
```
The previous code will print **JhonPork** and **Jhon Pork** respectively

Strings in python also work as 'arrays' like in Java, meaning we can take individual values from a String thanks to **indexing**
```python
city = 'Quito'
index = city[3]
print("Printing letter: " + idex) #this will print letter 't'
```

Now we can also use **negative indexing**, each index will always start by the end of the String as -1, this feature is useful, for example, when we want to get the character values of the last two letter imputed from users but we don't actually know how long the String will be, this way we always ensure we get the last characters without engineering too much

| index     | -5  | -4  | -3  | -2  | -1  |
| --------- | --- | --- | --- | --- | --- |
| character | Q   | u   | i   | t   | o   |
```python
city = 'Quito"
print(city[-1] + city[-2] + city[-3])
### this program will output "oti"
```

However when can achieve the same by using the **Len()** function
```python
city = 'quito'
last = city[len(city) - 1]
prev = city[len(city) - 2]
print('The last letter is ' + last + 'and the next after that is ' + prev)
# this will print "The last letter is o and the next after that is t"
```

## F-strings
We can further customise (format) how we want our output to look like. By placing variables and numbers inside our print function. This allows us to have more freedom with our outputs, specially useful when working with floating values

We can use this tool by placing an **f** inside the print argument and placing our variables and formats inside curly braces **{ }**

String variables example: 
```python
name = Jhon
age = 12
print(f"Hello my name is {name} and I am {age} years old")
```

Double variable example: 
```python
pi = 3.1416
print(f"The value of pi is: {pi:.1f}")
```

`:1,f` Meaning
	`:`    -> starts the format spec
	`.1` ->  one decimal place
	 `f`   -> highlight this is a floating number

#### String formatting options
##### 1. Alignment
We can align text to the left, centre, or right

| Format | Syntax      |
| ------ | ----------- |
| Left   | `:<[width]` |
| Right  | `:>[width]` |
| Center | `:^[width]` |
```python
name = "Alex"
print(f"My name is {name:<10}")
print(f"My name is {name:>10}")
print(f"My name is {name:^10}")
```
##### 2. Upper / Lower / Title Case
```python
name = "Alex"
print("My name is {name.upper()}") #ALEX
print("My name is {name.lower()}") #alex
print("My name is {name.title()}") #Alex
```
##### 3. Padding with custom characters
We can create padding with any character we'd like to use
```python
title = "Python"
print(f"{title:*^12}") #Output -> ***Python***
```
##### 4. Combining Formatting
```python
user = "Marie"
print(f"Welcome, {user.title():*^13}!") #Welcome, ****Marie****
```
