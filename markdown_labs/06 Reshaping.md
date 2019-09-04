# Reshaping Data – Lab
*Python for Data Science*

1. Load in the flights data that we've used before.

2. Using a pivot table, find the median flight time to go from each origin to each destination.
Save that resulting pivot table in a variable called "pivoted_df".

3. Experiment with the `.dropna` method -- consult its documentation using the `?`.
Use it to drop destinations in your result from #2 where at least one value is `NaN`.
Store this "cleaned" DataFrame in a variable called "clean_df".
    - destinations may be either rows or columns depending on how you did #2

4. Using your result from #3, extract the destination airport codes as a list.
What is the context of these airport codes?
i.e. When might it be helpful to have prepared a list of these airport codes?

5. Reload the planes data that we've used before.

6. Melt this data, using all columns except tailnum as your value variables.
Use tailnum as your identifier.
Store the result as "melted_df".

7. Use the .pivot method to "widen" the data from #6 and put it back in the form it started in.
    - The type and engine columns will be missing because we didn'

#### Challenge Questions
1. Using your result from #3 again, run the following code:
    - If your row labels (index) are **origin** airport: `clean_df.reset_index().melt(id_vars='origin', value_name='air_time').dropna()`
    - If your row labels are **dest**ination airport: `clean_df.reset_index().melt(id_vars='dest', value_name='air_time').dropna()`

2. Can you replicate the values in this resulting DataFrame using the original flights data and and performing a groupby and aggregate?
    - *Hint: passing `as_index=False` to `.groupby` will keep pandas from moving your grouping columns into the index, making your result look more like the data from #1.*

3. Do you have any intuition as to why this works?
