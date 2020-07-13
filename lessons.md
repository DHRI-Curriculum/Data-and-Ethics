# Data is Foundational

In this brief workshop we will be discussing the basics of research data, in terms of material, transformation, and presentation. We will also be focusing on the ethics of data cleaning and representation. Because everyone has a different approach to data and ethics, this workshop will also include multiple sites for discussions to help us think together as a group.

## What Constitutes Research Data?

"Material or information on which an argument, theory, test or hypothesis, or another research output is based."
[Queensland University of Technology. Manual of Procedures and Policies. Section 2.8.3.](http://www.mopp.qut.edu.au/D/D_02_08.jsp)

"What constitutes such data will be determined by the community of interest through the process of peer review and program management. This may include, but is not limited to: data, publications, samples, physical collections, software and models"
[Marieke Guy.](http://www.slideshare.net/MariekeGuy/bridging-the-gap-between-researchers-and-research-data-management)

"(i) Research data is defined as the recorded factual material commonly accepted in the scientific community as necessary to validate research findings, but not any of the following: preliminary analyses, drafts of scientific papers, plans for future research, peer reviews, or communications with colleagues."
[OMB-110, Subpart C, section 36, (d) (i)](http://www.whitehouse.gov/omb/circulars_a110/)

"The short answer is that we can’t always trust empirical measures at face value: data is always biased, measurements always contain errors, systems always have confounders, and people always make assumptions." [Angela Bassa](https://medium.com/@angebassa/data-alone-isnt-ground-truth-9e733079dfd4)

In summary, research data is:
**Material or information necessary to come to your conclusion.**

## Forms of Data

There are many ways to represent data, just as there are many sources of data. After processing our data, we turn it into a number of products. For example:

* Non-digital text (lab books, field notebooks)

* Digital texts or digital copies of text

* Statistical analysis (SPSS, SAS, R)

* Scientific sample collections

* Data visualizations

* Computer code

* Standard operating procedures and protocols

* Protein or genetic sequences

* Artistic products

* Curriculum materials

* Spreadsheets (e.g. .xlsx, .csv, .tsv)

* Audio (e.g. .mp3, .wav, .aac)

* Video (e.g. .mov, .mp4)

* Computer Aided Design/CAD (.cad)

* Databases (e.g. .sql)

* Geographic Information Systems (GIS) and spatial data (e.g. .shp, .dbf, .shx)

* Digital copies of images (e.g. .png, .jpeg, .tiff)

* Web files (e.g. .html, .asp, .php)

* Matlab files & 3D Models (e.g. .stl, .dae, .3ds)

* Metadata & Paradata (e.g. .xml, .json)

* Collection of digital objects acquired and generated during research

Adapted from: [Georgia Tech](http://libguides.gatech.edu/content.php?pid=123776&sid=3067221)

### Challenge: Forms of Data

These are some (most!) of the shapes your research data might transform into. 
1. What are some forms of data you use in your work? 
2. What about forms of data that you produce as your output? Perhaps there are some forms that are typical of your field. 
3. Where do you usually get your data from?

# Stages of Data

We begin without data. Then it is observed, or made, or imagined, or generated. After that, it goes through further transformations:

## Raw
    
Raw data is yet to be processed, meaning it has yet to be manipulated by a human or computer. Received or collected data could be in any number of formats, locations, etc.. It could be in any of the forms listed above.

But "raw data" is a relative term, inasmuch as when one person finishes processing data and presents it as a finished product, another person may take that product and work on it further, and for them that data is "raw data". 

## Data and Labor

As we think about data collection, we should also consider the labor involved in the process. Many researchers rely on Amazon Mechanical Turk (sometimes also refered to as MTurk) for data collection, [often paying less than minimum wage for the task.](https://www.theatlantic.com/business/archive/2018/01/amazon-mechanical-turk/551192/) Often the assumption made of these workers is someone who is retired, bored, and participating in online gig work for fun or to kill time. While this may be true for some, [more than half of those surveyed in a Pew Research study cite that the income from this work is essential or important.](https://www.pewresearch.org/internet/2016/11/17/labor-platforms-technology-enabled-gig-work/) Often, those who view the income from this work as essential or important are also from underserved communities. 

In addition to being mindful of paying a fair wage to the workers on such platforms, this working environment also brings some further considerations to the data that is collected. Often times, for workers to get close to minimum wage, they cannot afford to spend much time on each task, increasing potential errors in the collected data. 

### Challenge: Raw Data and Labor

1. For example, is "big data" "raw data"? How do we understand data that we have "scraped"? 

## Processed/Transformed

Processing data puts it into a state more readily available for analysis, and makes the data legible. For instance it could be rendered as **structured data**. This can also take many forms, e.g., a table. 

Here are a few you're likely to come across, all representing the same data:

**XML**

```xml
<Cats> 
    <Cat> 
        <firstName>Smally</firstName> <lastName>McTiny</lastName> 
    </Cat> 
    <Cat> 
        <firstName>Kitty</firstName> <lastName>Kitty</lastName> 
    </Cat> 
    <Cat> 
        <firstName>Foots</firstName> <lastName>Smith</lastName> 
    </Cat> 
    <Cat> 
        <firstName>Tiger</firstName> <lastName>Jaws</lastName> 
    </Cat> 
</Cats> 
```

**JSON**

```json
{"Cats":[ 
    { "firstName":"Smally", "lastName":"McTiny" }, 
    { "firstName":"Kitty", "lastName":"Kitty" }, 
    { "firstName":"Foots", "lastName":"Smith" }, 
    { "firstName":"Tiger", "lastName":"Jaws" } 
]} 
```

**CSV**

```csv
First Name,Last Name/n
Smally,McTiny/n
Kitty,Kitty/n
Foots,Smith/n
Tiger,Jaws/n
```

### The importance of using open data formats

A small detour to discuss (the ethics of?) data formats. For accessibility, future-proofing, and preservation, keep your data in open, sustainable formats. A demonstration:

1. Open [this file](cats.csv) in a text editor, and then in an app like Excel. This is a CSV, an open, text-only, file format.
2. Now do the same with [this one](cats.xlsx). This is a proprietary format! 

Sustainable formats are generally unencrypted, uncompressed, and follow an open standard. A small list:

* ASCII

* PDF 

* .csv

* FLAC

* TIFF

* JPEG2000

* MPEG-4

* XML

* RDF

* .txt

* .r

### Challenge: Processed/Transformed

How do you decide the formats to store your data when you transition from 'raw' to 'processed/transformed' data? What are some of your considerations?

## Tidy Data

There are guidelines to the processing of data, sometimes referred to as **Tidy Data**.<sup>1</sup> One manifestation of these rules:
1. Each variable is in a column.
2. Each observation is a row.
3. Each value is a cell.

Look back at our example of cats to see how they may or may not follow those guidelines. **Important note**: some data formats allow for more than one dimension of data! How might that complicate the concept of **Tidy Data**?

```json
{"Cats":[
    {"Calico":[
    { "firstName":"Smally", "lastName":"McTiny" },
    { "firstName":"Kitty", "lastName":"Kitty" }],
    "Tortoiseshell":[
    { "firstName":"Foots", "lastName":"Smith" }, 
    { "firstName":"Tiger", "lastName":"Jaws" }]}]}
```

 <sup>1</sup>Wickham, Hadley. "Tidy Data". Journal of Statistical Software.


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
    
**Validity**  

Measurements must be valid, in that they must conform to set constraints:
1. The aforementioned "yes" or "y" or "1" should all be changed to one response.
2. Certain fields cannot be empty, or the whole observation must be thrown out.
3. Uniqueness, for instance no two people should have the same social security number.
    
**Accuracy**  

Measurements must be accurate, in that they must represent the correct values. While an observation may be valid, it might at the same time be inaccurate. 123 Fake street is a valid, inaccurate street address.
Unfortunately, accuracy is mostly acheived in the observation process. To be achieved in the cleaning process, an outside trusted source would have to be cross-referenced.

**Completeness**

Measurements must be complete, in that they must represent everything that might be known. This also is nearly impossible to achieve in the cleaning process! For instance in a survey, it would be necessary to re-interview someone whose previous answer to a question was left blank. 
    
**Consistency**  

Measurements must be consistent, in that different observations must not contradict each other. For instance, one person cannot be represented as both dead and still alive in different observations. 
    
**Uniformity**  

Measurements must be uniform, in that the same unit of measure must be used in all relevant measurements. If one person's height is listed in meters and another in feet, one measurement must be converted.

### Challenge: When do we stop cleaning?  

How do we know when our data is cleaned enough? What happens to the data that is removed? What are we choosing to say about our dataset as we prepare them for analysis?

## Analyzed

Analysis can take many forms (just like the rest of this stuff!), but many techniques fall within a couple of categories:

### Descriptive Analysis

Techniques geared towards summarizing a data set, such as:

* Mean

* Median

* Mode

* Average

* Standard deviation

### Inferential Analysis

Techniques geared towards testing a hypothesis about a population, based on your data set, such as:

* Extrapolation

* P-Value calculation

### Challenge: Analysis

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

### Challenge: Visualizations

As we transform our results into visuals, we are also trying to tell a narrative about the data we collected. Data visualization can help us to decode information and share quickly and simply. What are we assuming when we choose to visually represent data in particular ways? How can data visualization mislead us?

# Data Literacy and Ethics

Throughout the workshop we have been thinking together through some of
the potential ethical concerns that might crop up as we proceed with our
own projects. Just as we have disucssed thus far, we hope that you see
that data and ethics is an ongoing process throughout the lifespans of
your project(s) and don’t often come with easy answers.

## Activity

In this final activity, we would like for you to think about some of the
potential concerns that might come up in the scenario below and discuss
how you might approach them:

You are interested in looking at the reactions to the democratic party
presidential debates across time. You decided that you would use data
from twitter to analyze the responses. After collecting your data, you
learned that your data has information from users who were later banned
and included some tweets that were removed/deleted from the site.

### If you would like some guiding questions:

  - Would your approach differ if the responses were anonymized v. not?
  - Would the number of tweets generated impact your decisions?
  - How might where you are at in your project (e.g. "raw" data v. "cleaned" data v. analysed) affect your choices?

## Some concluding thoughts

Data and ethics are contextually driven. As such, there isn’t always a
risk-free approach. We often have to work through ethical dilemmas while
thinking through information that we may not have (what are the risks of
doing/not doing this work?). We may be approaching a moment where the
question is no longer what we could do but what we should do.








