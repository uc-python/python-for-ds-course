# Joining Data – Lab
*Python for Data Science*

1. You should have already downloaded the planes data ([https://raw.githubusercontent.com/uc-python/intro-python-datasci/master/data/planes.csv](https://raw.githubusercontent.com/uc-python/intro-python-datasci/master/data/planes.csv)).
Now download a related dataset – flights data ([https://raw.githubusercontent.com/uc-python/intro-python-datasci/master/data/flights.csv](https://raw.githubusercontent.com/uc-python/intro-python-datasci/master/data/flights.csv)).
Note that this is a fairly large dataset and may take a few seconds to download.

2. Load in the planes data as `planes` and the flights data as `flights`.

3. Inspect the flights data with the tools you've learned so far -- methods like `.head` and `.describe`, attributes like `.shape` and `.dtypes`.
Based on what you see in the dataset, form a hypothesis about what this dataset is.
Do you see a column in this data that could match up with a column in the planes data?

4. Just using the flights data, is it possible to determine what percentage of the flights were completed on Boeing planes?
Why not?

5. In order to combine this data with the planes data (where the manufacturer column is), we need to do a join.
Inner join the planes data to the flights data, storing the result in a variable called `joined_data`.
You'll need to determine the column that makes sense to join on.

6. How many rows are in the result DataFrame?
How does this compare to how many rows were in its parent DataFrames (planes and flights)?

7. What would happen if you did a left join instead of an inner join?
Try it, storing the result in a variable called `left_joined_data`.
Check how many rows are in this new DataFrame -- why is it different to the number of rows in `joined_data` (from #5)?

8. Using the original (inner) joined data, calculate what percentage of flights were completed on Boeing planes.
