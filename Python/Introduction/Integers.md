Integers work mostly the same as other programming languages as Java

They represent whole numbers bot positive and negative

Contrary to languages like Java, we aren't obligated to specify the type of variable we are assigning so we can do this:

```python
name = 'Pierre'  #string
age = '50'       #int
```

However, its important to highlight the type of variable when concatenating then into a string output
```python
print('Hello my name is ' + name)
print('I am ' + str(age) + 'years old')
```

If we forget to cast `str()` into `age` we will get a compilation issue as concatenating pure integer values with strings is not possible in Python

Something similar must be done when working with inputs
```python
revenue = int(input('Business revenue: '))
cost = int(input("Business cost: "))
profit = revenue - cost
print('Your total profit is: ' + str(profit))
```

If we forget to cast `int()` into our input, the values typed will be registered as String values, making the profit maths operation fail as we cannot subtract string values from one another, at least not in the maths sense 