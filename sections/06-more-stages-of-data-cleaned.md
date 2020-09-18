← [Side Note on Data Structures: Tidy Data](05-side-note-on-data-structures-tidy-data.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[More Stages of Data: Analyzed](07-more-stages-of-data-analyzed.md) →

---

# 6. More Stages of Data: Cleaned

High quality data is measured in its **validity**, **accuracy**, **completeness**, **consistency**, and **uniformity**.

Processed data, even in a table, is going to be full of errors:

1. Empty fields
2. Multiple formats, such as "yes" or "y" or "1" for a positive response.
3. Suspect answers, like a date of birth of 00/11/1234
4. Impossible negative numbers, like an age of "-37"
5. Dubious outliers
6. Duplicated rows
7. And many more!

Cleaning data is the work of correcting the errors listed above, and moving towards high quality. This work can be done manually or programmatically.

### Validity

Measurements must be valid, in that they must conform to set constraints:

1. The aforementioned "yes" or "y" or "1" should all be changed to one response.
2. Certain fields cannot be empty, or the whole observation must be thrown out.
3. Uniqueness, for instance no two people should have the same social security number.

### Accuracy

Measurements must be accurate, in that they must represent the correct values. While an observation may be valid, it might at the same time be inaccurate. 123 Fake street is a valid, inaccurate street address.

Unfortunately, accuracy is mostly achieved in the observation process. To be achieved in the cleaning process, an outside trusted source would have to be cross-referenced.

### Completeness

Measurements must be complete, in that they must represent everything that might be known. This also is nearly impossible to achieve in the cleaning process! For instance in a survey, it would be necessary to re-interview someone whose previous answer to a question was left blank.

### Consistency

Measurements must be consistent, in that different observations must not contradict each other. For instance, one person cannot be represented as both dead and still alive in different observations.

### Uniformity

Measurements must be uniform, in that the same unit of measure must be used in all relevant measurements. If one person's height is listed in meters and another in feet, one measurement must be converted.

## Evaluation

Measurements are *accurate* when
- observations do not contradict each other.
- they represent the correct values.*
- when they are unique responses (e.g. no duplication).
- when the same unit of measure is used in all relevant measurements.

## Challenge: When Do We Stop Cleaning?

1. How do we know when our data is cleaned enough?
2. What happens to the data that is removed?
3. Explore the `moSmall.csv` dataset.
    - Are all the measurements valid? Try checking the `Object ID` column for duplicates.
    - How might you check if the `Is Public Domain` accurately represents the copyrights of the media objects?
    - Is the data collected completed? How might you deal with the NA or empty fields?
        - What assumptions do you have to make when you clean NA or empty fields?
    - Is the collected data consistent? Does the column `Is Public Domain` correspond with the data in `Rights and Reproduction`? If it does not, which would you follow? Why?
    - As the dataset is not one that we personally collected, how do we make sense that only `Female` or `|` is collected as responses in the column (with the exception of NA and empty fields)? What do we have to do to the data to make sure it is uniform? What decisions do we make in this process?

## Solution:

1. I think this is often decided before the cleaning process begins, perhaps after some quick visualization or analysis of the "raw" data. I generally remove empty entries from my data sets. Working with social media data, I also usually remove URLs as these influence the topic modelling algorithms (e.g. "http" may end up being the most prominent topic of the corpus). This is usually where I stop cleaning. Some might suggest the removal of stop words like "the" "a" "an," but I have always felt very uncertain about the removal of these words. This is especially because the dictionary of stop words were generated through canon western texts that is not representative of the many variations of English. For example, if I were looking at the tweets of Singaporean youths, the stop word dictionary may not be appropriate.
2. For me, the data is often destroyed (usually because IRB desires it) or it remains in the original "raw" file. The file that I clean will always be a duplicate file to allow for recovery in case I made a poor decision in the process of cleaning.
3. Exploring the dataset, here are my responses to the questions:
    - Using `Object ID` indicates that there is no duplicates in the dataset. Every entry is unique.
    - I will have to compare it to another trusted source like a database from [The Getty Research Institute](https://www.getty.edu/research/tools/).
    - The data collected is not completed. There are missing fields. Depending on where the missing field is, I may choose to code it as `0` for the ease of analysis. For example, the column `Dynasty` only contain 1 meaningful entry within this sample data set, as such, I will not run any analysis that may rely on this column and choose to drop it. The column `Accession Year` only has 1 NA and I will choose to drop that row if this becomes a useful variable for my analysis.
    - While the `Rights and Reproduction` contains a lot of NA and inappropriate responses (e.g. "Ceramics"), for the most part, for the items labeled as `YES` in the column `Is Public Domain` the corresponding column in `Rights and Reproduction` does not record a copyright holder. I am assuming that the NA can stand in for the object being in the public domain.
    - Taking only `Female` as a valid gender response, everything else will be converted to a `0` for ease of analysis. I am assuming `|` as equivalent to a NA or an empty field rather than an alternative gender. Hence in my analysis, the proportion will only record female artists' objects against the rest of the collected items. I cannot necessarily answer the larger question of all non-cisgender men against the total in this case.

---

← [Side Note on Data Structures: Tidy Data](05-side-note-on-data-structures-tidy-data.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[More Stages of Data: Analyzed](07-more-stages-of-data-analyzed.md) →