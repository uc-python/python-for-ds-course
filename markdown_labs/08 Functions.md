# Functions – Lab
*Python for Data Science*

1. The formula for the circumference of a circle is *2 * pi * radius*.
Write a function, `calculate_circumference`, that accepts a `radius` argument and returns the circumference of a circle with that radius.
*Hint: use `pi` from the `math` library.*

2. Update your function from #1 -- make the radius parameter default to 1.

3. Create a list, `radii`, `[4, 83, 3.7, 9]`.
Loop over these elements and use your function from #1 to check the circumference for each radius in that list.

4. Rewrite your function from #1 (without a default argument) as a lambda function.

5. Repeat #3, but using your lambda function instead.
Is anything different about your results?

6. Create a function `caller` that accepts two arguments: `func` and `target`.
Implement the body of `caller` so that it takes calls the input function (`func`) on the input target (`target`) and returns the result.
e.g. `caller(type, 7)` would be the same as `type(7)`, returning `int`.

7. Create a function, `nan_filler`, that takes as arguments a DataFrame and a scalar value. Implement it to return a copy of that DataFrame with all `NaN`s replaced with the scalar value.

8. Copy the below function defintion to your notebook and try calling it with different inputs.
Pass it a single positional argument, several positional arguments, a single keyword argument, several keyword arguments, and then a mix of positional and keyword arguments.
Form a hypothesis about how `*args` and `**kwargs` work.
```python
def weird_func(*args, **kwargs):
    print('args', args)
    print('kwargs', kwargs)
```