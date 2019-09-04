# Python – Lab
*Python for Data Science*

1. What is the difference between Python and Jupyter?
Type a comment in your notebook explaining the difference.

2. 4k monitors are 3840 pixels wide and 2160 pixels tall.
Assign these values to variables called `width` and `height`.

3. Check the values of these variables by printing them.

4. Create a new variable, `total_pixels`, and assign it the product of *height* and *width*.

5. What type of data is in `total_pixels`? (int, float, string, boolean).
Use the `type` function to check.

6. Create variables `first_name` and `last_name` and in them, store your given name and surname, respectively.
Use the `+` operator to "add" these together to form your full name.
*Hint: You may realize you need to add another character in between them.*

7. Copy and run the following code.
```python
mystery = [{'abc': 'def'}]
```
What type of data is `mystery`?
Use the `type` function to check.

8. What type of data is the first element of `mystery`?
*Hint: You'll need to use brackets to access an element by its location. And don't forget Python starts counting at 0!*

9. Run the below code.
```python
import pandas as pd
df = pd.DataFrame([['Coffee', 310], ['Tea', 90]],
                  columns=['beverage', 'caffeine'])
```
What type of data is in the `df` variable?

10. Take a look at the arguments we passed into `pd.DataFrame` in #9.
There are two.
What is the type of each of them?

11. What would have happened if we hadn't imported Pandas in #8?
Run `del pd` to delete the name `pd` from Python's memory, and then run the rest of the code (`df = pd.DataFrame...`) again to see.

12. Import Pandas again, under the alias `pd` (as before).
Use `type` to check -- what type of data is in `pd`?