# Grouping Data – Lab
*Python for Data Science*

1. Reload the `planes` and `flights` DataFrames, from the last lab.

2. What is the average departure delay (`dep_delay`) of all flights in this data?

3. What is the average departure delay by carrier, for flights in this data?

4. If you followed the groupby-agg workflow we covered in lecture, you passed your summary function within a list.
Try removing the brackets and rerunning #3.
What's different about the result?
Why do you think we focused on the list-based approach in class?

5. Working from your code for #3, calculate the minimum, mean, median, and maximum departure delay for each carrier.
Don't do this in 4 separate lines -- you can achieve this result using a single invocation of `groupby` and a single invocation of `agg`.

6. Perhaps, after doing some research, you discover that the most meaningful statistic for departure delay is the *average delay*, but the most meaningful way to measure air time is the *median air time*.
Build a groupby-agg invocation that summarizes – at the carrier level – the average departure delay and the median air time.

7. What is the single most common route in this data?
That is to say, what combination of values for `origin` and `destination` occurs most frequently? *Hint: to order the data yourself, you may want to experiment with the `sort_values` method of Pandas Series.*

#### Challenge question

Same as #7, but by carrier: what route is most common for each carrier? You will need to use approaches beyond what we've seen in class, but you should be able to find code that gets you most of the way there just by googling.