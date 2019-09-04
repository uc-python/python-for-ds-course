# DataFrames – Lab
*Python for Data Science*

*Note: Some of these exercises may also require you to consult the lecture on importing & exporting.*

1. Download the dataset at [https://raw.githubusercontent.com/uc-python/intro-python-datasci/master/data/planes.csv](https://raw.githubusercontent.com/uc-python/intro-python-datasci/master/data/planes.csv) and load it into Python as a DataFrame.
Store it in a variable called `df`.

2. Print the first few rows of the DataFrame using the `.head()` method of `df`.

3. Take a look at a few attributes of `df`: `.shape`, `.index` and `.columns`.
Do the contents of these attributes give you any information about the DataFrame?

4. Check the data types of the columns of `df`. *Hint: We did this during lecture in one of the early slides.*

5. Select just the `year` column using `df['year']`. Store the result in a variable called `year`. Print it out.

6. What is the type of `year`?

7. Select *both* the `manufacturer` and `model` columns and store the result in a variable called `plane_types`. Print it out.

8. What is the type of `plane_types`? Why is this different from #6?

9. Slice the row at index 105. What year was this plane made?

10. Filter down the dataset to only planes made by Boeing. How many rows are left? *Hint: Use `.shape` to get a row count.*

11. In the filtered data from #10, what do you notice about the indexes? Call the `.reset_index()` method on this data and see what changes.

12. How many planes in the data have fewer than 40 seats?

13. What is the minimum number of seats of any plane in the data? *Hint: This is a good time to use summary functions.*

14. What is the minimum number of seats in any plane made by Boeing?

15. Create a new column in `df` called `seats_per_engine`. It is defined as number of seats divided by number of engines.

16. What is the average (mean) number of seats per engine in the data?

17. Create a subset of the data, containing only planes manufactured by Cessna. Select all the columns *except* manufacturer (since we know they're all Cessna). Export the data as a CSV called "cessna_planes.csv".