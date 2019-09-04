# Apply – Lab
*Python for Data Science*

1. Write a transforming function implementing the formula `y = 5x - 2`

2. Create a numeric Pandas Series using the `pd.Series` call we've seen before. Use values of your choice.

3. Apply your transforming function from #1 to this Series.

4. Repeat #3, but apply `y = 5x - 2` as a lambda function instead of a *named* function.

5. Apply this lambda function to your Series: `lambda x: [x, x + 1]`.
What type of data is now in each element?
Why did that happen?

6. Open the flights data.
Create and apply a function such that the result is a Series with one element for each row.
*Hint: take a look at the chart from lecture.*

7. Create a function that takes in a row (a Series) and returns a string with "carrier" and "flight" combined together into one, separated by a dash. I.e. running your function on the first row should yield "UA-1545".

8. Apply your function from #7 to every row, and use it to create a new column "carrier_flight_code".

9. Suppose we learn that there are some systematic errors in the data. "dep_delay" is understated by two minutes for all flights leaving from LGA and overstated by 1 minutes for flights leaving from EWR.
It's correct for flights leaving from JFK.
Use a custom function and an `apply` to create a new column, "real_dep_delay", adjusting for these inaccuracies.

10. Subset your flights data to the first 10,000 rows -- the next question is fairly computationally intense, and this will make it run faster.

11. You've been assigned to summarize the data in a very particular way:
get the modal value of columns whose names start with "dep", and get the mean value of columns whose names start with "arr".
Do this using an applied function.
*Hint: remember you can check the name of a Series using its `.name` attribute*

12. How could you have done this without `apply`?
There are a few ways.
Are any as concise as `apply`?