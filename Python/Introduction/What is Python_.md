Computer languages are more precise and there are less rules-exceptions to be worried about, contrary to human language. Still python is a high level language with a code syntax  similar to the English

This program is used to determine if a US citizen need to get a new passport or not
```python
   import time
   current_year = int(time.strftime('%Y'))
  received_year = int(input('What year did you get your passport? '))
   if received_year + 10 < current_year:
       print('You should go get a new passport')
   else:
       print('You may use your current passport')
````

- Line 1: we let to know the computer that we need information about time
- Line 2: save the current year by the name **current_year
- Line 3: asks whoever is using the program to enter the year of the passport
- Line 4: check if the passport is valid and then checks a loop

This code uses simple tasks such as [[Input and Output]]

Reference
[[Methods]]
[[Variables]]

