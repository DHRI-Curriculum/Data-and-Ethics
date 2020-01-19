[<<< Previous](stages.md) | [Next >>>](discussion.md)

# More Stages of Data

## Cleaned
    
High quality data is measured in its **validity**, **accuracy**, **completeness**, **consistency**, and **uniformity**.

Processed data, even in a table, is going to be full of errors:
1. Empty fields
2. Multiple formats, such as "yes" or "y" or "1" for a positive response.
3. Suspect answers, like a date of birth of 00/11/1234
4. Impossible negative numbers, like an age of "-37"
5. Dubious outliers
6. Duplicated rows
7. And many more!

Cleaning data is the work of correcting the errors listed above, and moving towards high quality. This work can be done manually or programatically. 
    
#### Validity
Measurements must be valid, in that they must conform to set constraints:
1. The aforementioned "yes" or "y" or "1" should all be changed to one response.
2. Certain fields cannot be empty, or the whole observation must be thrown out.
3. Uniqueness, for instance no two people should have the same social security number.
    
#### Accuracy
Measurements must be accurate, in that they must represent the correct values. While an observation may be valid, it might at the same time be inaccurate. 123 Fake street is a valid, inaccurate street address.
Unfortunately, accuracy is mostly acheived in the observation process. To be achieved in the cleaning process, an outside trusted source would have to be cross-referenced.

#### Completeness
Measurements must be complete, in that they must represent everything that might be known. This also is nearly impossible to achieve in the cleaning process! For instance in a survey, it would be necessary to re-interview someone whose previous answer to a question was left blank. 
    
#### Consistency
Measurements must be consistent, in that different observations must not contradict each other. For instance, one person cannot be represented as both dead and still alive in different observations. 
    
#### Uniformity
Measurements must be uniform, in that the same unit of measure must be used in all relevant measurements. If one person's height is listed in meters and another in feet, one measurement must be converted.

### Discussion: When do we stop cleaning?
How do we know when our data is cleaned enough? What happens to the data that is removed? What are we choosing to say about our dataset as we prepare them for analysis?

## Analyzed

Analysis can take many forms (just like the rest of this stuff!), but many techniques fall within a couple of categories:

#### Descriptive Analysis

Techniques geared towards summarizing a data set, such as:

* Mean

* Median

* Mode

* Average

* Standard deviation

#### Inferential Analysis

Techniques geared towards testing a hypothesis about a population, based on your data set, such as:

* Extrapolation

* P-Value calculation

### Discussion: Analysis
As we consider the types of analysis that we choose to apply onto our data set, what are we representing and leaving out? How do we guide our decisions of interpretation with our choices of analyses? Are we comfortable with the intended use of our research? Are we comfortable with the unintended use of our research? What are potential misuses of our outputs? What can happen when we are trying to just go for the next big thing (tool/methods/algorithms) or just ran out of time and/or budget for our project?


## Visualized

* Comparisons
    * bar & line
    * side-by-side bars
    * dot plot
    * scatter plot
* Time
    * dot plot
    * slope graph
    * line graph
    * sankey diagram
    * timeline
* Small numbers/percentages
    * pie chart
    * tree map
    * waterfall
* Survey responses
    * bar chart
    * stacked bar
    * nested map
* Place
    * chloropleth map
    * hex or tile map

Adapted from Evergreen, Stephanie D. Effective data visualization : the right chart for the right data. Los Angeles: SAGE, 2017.

### Discussion: Visualizations
As we transform our results into visuals, we are also trying to tell a narrative about the data we collected. Data visualization can help us to decode information and share quickly and simply. What are we assuming when we choose to visually represent data in particular ways? How can data visualization mislead us?

[<<< Previous](stages.md) | [Next >>>](discussion.md)
