# Control Flow – Lab
*Python for Data Science*

1. The Python built-in function `input` prompts the user to enter text.
Use the `input` function to ask the user for his or her age (you may need to google it or look at docs for examples).
If the user's age is less than 13, print a message telling them that they are a child.
If the user's age is between 13 and 19, print a message telling them that they are a teenager.
If the user is 20 or over, tell them they are old.
*Hint: you may want to use the `int()` function to coerce strings to integers.*

2. Using the planes DataFrame, loop through the values in the engine column and count how many contain a dash (-).
You may want to use the `in` operator to check if one string is inside another.

3. Loop through every row in the planes DataFrame (try `df.iterrows()`) and sum up the number of engines *until* you encounter a plane made by Boeing.

4. The fizzbuzz problem (a famous coding interview question):
    - Loop through the integers from 1 to 100
    - For any number divisible by 3, print 'fizz'
    - For any number divisible by 5, print 'buzz'
    - For any number divisible by both 3 and 5, print 'fizzbuzz'
    - For all other numbers, just print the number

5. Fill in the blanks in this list comprehension to produce the output [1, 3, 5]:
```python
[x * _ + _ for x in range(3)]
```

6. Given a list `l = [4, 5, 2, 0, 2]`, write a list comprehension that produces `[12, 15, 6, 0, 6]`:
```python
[ _____ for _ in l]
```

7. Write a list comprehension that returns a list of the columns of `planes` in all caps. *Hint: use `planes.columns` in the comprehension.*