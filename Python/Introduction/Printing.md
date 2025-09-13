Printing messages to the console can we done with:
`print('the big black box')`

[[print()]] is one of many [[Python/Introduction/Functions]] that are built inside Python.

The text enclosed within quotes is referred as a string. [[Strings]] can be used to print any kind of text

Example:

````python
print("the")
print('big')
print("black")
print('box')
````
 the output will be:
 ```python
 the
 big
 black
 box
```

By default the *print()* function adds a special character at the end of each string better known as the **newline** character

Its a break, like hitting Enter

Example:
```python
print("the\nbig\nblack\nbox")
```

Or we can instruct not to use a **newline**
```python
print("the", end=' ')
```

For printing string that spans multiple lines we must use triple quotes `'''` or we will get a compilation error
```python
#this wont work
print('the
big
black
box')

#################

#this will work
print('''the
big
black
box''')
```

Although text is not the only thing we can print, we could use [[Variables]] and [[Concatenation]]

Using variables is useful when we need to use the same information/data over and over again in our code
```python
character_1 = 'John'
character_2 = 'Luke'

print(character_1 + ': Hi ' + character_2 + ', long time since we talked last.')
print(character_2 + ': Hi ' + character_1 + '! How have you been?')
print(character_1 + ': I have been well. Do you wanna go get lunch?')
print(character_2 + ': Yes!')
print(character_1 + ': Great, we can meet at In-n-Out burger next week')
```
In the previous example the characters names where mentioned more than once, writing their names would not be a problem in this case, but if our text would be 1000th pages long, changing the names would be quite the task.

Contrary to just re-naming one String variable

String concatenation can also be done by placing a '**,**' in front of our variables, and it will create a 'natural space' in the output, instead of jamming the string together without using a '**+**'
```python
value_1 = 'bear'
value_2 = 'deer'
Print(value_1, value_2)

#this will print -> bear deer
```
