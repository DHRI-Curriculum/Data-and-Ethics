# Data is Foundational

In this brief workshop we will be discussing the basics of research data in terms of material, transformation, and presentation. We will also be discussing the complicated ethics of data collection, cleaning, and representation. Because everyone has a different approach and understanding to data and ethics, this workshop will also include multiple sites for discussions to help us think through what data literacy means within our projects and broader applications.

## What Constitutes Research Data?

These quotes below offers a variety of perspectives to understanding research data across different stakeholders. The inclusion of these different approaches to research data is to suggest that there is no singular, definitive approach, and is dependent on multiple factors, including your project considerations. 

"Material or information on which an argument, theory, test or hypothesis, or another research output is based."
[Queensland University of Technology. Manual of Procedures and Policies. Section 2.8.3.](http://www.mopp.qut.edu.au/D/D_02_08.jsp)

"What constitutes such data will be determined by the community of interest through the process of peer review and program management. This may include, but is not limited to: data, publications, samples, physical collections, software and models."
[Marieke Guy](http://www.slideshare.net/MariekeGuy/bridging-the-gap-between-researchers-and-research-data-management)

"(i) Research data is defined as the recorded factual material commonly accepted in the scientific community as necessary to validate research findings, but not any of the following: preliminary analyses, drafts of scientific papers, plans for future research, peer reviews, or communications with colleagues."
[OMB-110, Subpart C, section 36, (d) (i)](http://www.whitehouse.gov/omb/circulars_a110/)

"The short answer is that we can’t always trust empirical measures at face value: data is always biased, measurements always contain errors, systems always have confounders, and people always make assumptions." [Angela Bassa](https://medium.com/@angebassa/data-alone-isnt-ground-truth-9e733079dfd4)

Broadly, research data can be understood as **materials or information necessary to come to your conclusion** but what these materials and information is depends on your project. 

## Forms of Data

There are many ways to represent data, just as there are many sources of data. What can you/do you count as data? Here's a small list of possibilities: 

- Non-digital text (lab books, field notebooks)
- Digital texts or digital copies of text
- Statistical analysis (SPSS, SAS, R)
- Scientific sample collections
- Data visualizations
- Computer code
- Standard operating procedures and protocols
- Protein or genetic sequences
- Artistic products
- Curriculum materials (e.g. course syllabi)
- Spreadsheets (e.g. .xlsx, .csv, .tsv)
- Audio (e.g. .mp3, .wav, .aac)
- Video (e.g. .mov, .mp4)
- Computer Aided Design/CAD (.cad)
- Databases (e.g. .sql)
- Geographic Information Systems (GIS) and spatial data (e.g. .shp, .dbf, .shx)
- Digital copies of images (e.g. .png, .jpeg, .tiff)
- Web files (e.g. .html, .asp, .php)
- Matlab files & 3D Models (e.g. .stl, .dae, .3ds)
- Metadata & Paradata (e.g. .xml, .json)
- Collection of digital objects acquired and generated during research

Adapted from: Georgia Tech

## Challenge: Forms of Data

These are some (most!) of the shapes your research data might transform into. 

1. What are some forms of data you use in your work? 
2. What about forms of data that you produce as your output? Perhaps there are some forms that are typical of your field. 
3. Where do you usually get your data from?

- - - 
## Example Solution: Forms of Data
1. As I am currently exploring discourses on various social media ecosystem, I tend to extract/scrape data that comes through as JSON files, which is a text-file type that is often used to structure large data sets. Sometimes they also come in other forms of data bases such as CSVs or XLS. 
2. Often times outputs are statistical analysis and various data visualizations. This is also pretty comment in my field of psychology. 
3. I can get them from large databases like pushshift.io or scrape certain social media outlets directly such as Twitter. 

# Stages of Data

We begin without data. Then it is observed, or made, or imagined, or generated. After that, it goes through further transformations. For example, we can consider the stages in the following way:   
- We start with formulating a research question(s) or hypotheses and set up a project to answer our question(s). 
    - E.g. What have young voters in Singapore discussed in the weeks leading up to the election? 
- In the process of setting up the project, we make decisions on what kind of data we think can help us to answer the question 
    - E.g. I think I can get the data from Twitter where young folx are engaging in political conversations online. I will search a set of keywords and hashtags to collect a set of data for analysis. 
- After collecting our data we then consider and make decisions in the processes of cleaning. 
    - E.g. removing empty fields, coding particular responses as 1 or 0s
- We then run our preliminary analysis of the data. 
    - E..g. topic modelling to look at themes that emerge from the corpus.
- At the end of our analysis, a decision is then made about how would we would present the data and its analysis. 
    - E.g. is a word cloud useful to represent prevelant themes? Maybe a bar chart of proportion across the entire corpus?

This is one cycle in which data goes from collection to transformation to visualization. This is also *not* the only way to go through the stages. For example, we could do a preliminary analysis first, such as running a correlation of variables, to explore what is missing before we begin the process of cleaning. Often, we also end up doing multiple iterations of cleaning and analysis, making decisions and choices to collapse particular variables or remove them entirely at each iterations. Making sure that we keep a clear documentation of our process will ensure that we are accountable to the data we have collected/are using and also ensure that our results can be replicated and reproduced if others choose to work on our "raw" data.

## Raw
    
"Raw" data is yet to be processed, meaning it has yet to be manipulated by a human or computer. Received or collected data could be in any number of formats, locations, etc.. It could be in any of the forms listed in the previous section.

But "raw" data is a relative term, inasmuch as when one person finishes processing data and presents it as a finished product, another person may take that product and work on it further, and for them that data is "raw" data. For example, I may consider the [General Social Survey](http://gss.norc.org/) data to be "raw" as it will require me to filter out missing entries and collapse variables or fields before I can run my analysis. A researcher who participated in the creation of this survey may not consider the version on the site as "raw" because the "raw" version is the physical paper copies of the file. As you can see, this consideration of what is "raw" is non-definitive and is dependent on the project you are working on and the narrative you want to tell with the results. 

If you are interested in further exploration and discussion of the ethics of "raw" data, please consider reading [Drucker's article](http://www.digitalhumanities.org/dhq/vol/5/1/000091/000091.html) who has made useful distinctions between "data" (understood as given) and "capta (taken or "captured") that also troubles the distinction between "raw" and "processed" data. 

## Data and Labor

As we think about data collection, we should also consider the labor involved in the process. Many researchers rely on Amazon Mechanical Turk (sometimes also refered to as MTurk) for data collection, [often paying less than minimum wage for the task.](https://www.theatlantic.com/business/archive/2018/01/amazon-mechanical-turk/551192/) Often the assumption made of these workers is someone who is retired, bored, and participating in online gig work for fun or to kill time. While this may be true for some, [more than half of those surveyed in a Pew Research study cite that the income from this work is essential or important.](https://www.pewresearch.org/internet/2016/11/17/labor-platforms-technology-enabled-gig-work/) Often, those who view the income from this work as essential or important are also from underserved communities. 

In addition to being mindful of paying a fair wage to the workers on such platforms, this working environment also brings some further considerations to the data that is collected. Often times, for workers to get close to minimum wage, they cannot afford to spend much time on each task, increasing potential errors in the collected data. 

For a deeper discussion on data and labor, consider Catherine D'Ignazio and Lauren Klein's chapter [Show Your Work](https://mitpressonpubpub.mitpress.mit.edu/pub/9m0tiz66/release/3) in *[Data Feminism](https://mitpress.mit.edu/books/data-feminism)*.

## Challenge: Raw Data and Labor

1. Do you think "big data" is "raw data"? Why or why not? Do quantity of data play into our assumptions of "rawness"?
2. How should we approached data that we have "scraped"? 
3. How do you collect "raw" data? What are some of your practices? What are your field's practices?

- - - 
## Example Solution: Raw Data and Labor
1. I think big data can be raw data depending on how the data is obtained and the processes I need to take before I can apply an analysis. I think that with large datasets, I always assume "rawness" because I won't need all of the variables or there will be decisions that need to be made about missing entries. 
2. I think my approach to scraped data is similar to big data. 
3. Currently I collect through either pushshift.io or scrap permissible social media sites on my own or with my collaborator (who will have appropriate authorship). I know that my field of psychology is guilty of the discussion on mechanical turk and also often rely on undergraduates for experimental data collection who would have to sign up for experiments for credits in class or do the labour of working in the lab for the promises of bettering their resume for grad school applications. 

## Processed/Transformed

Processing data puts it into a state more readily available for analysis and makes the data legible. For instance, it could be rendered as **structured data**. This can also take many forms, _e.g._, a table. Other common examples of file types you are likely to come across are (they all represent the same data!):

XML: Or eXstensible Markup Language, uses a nested structure, where the "tags" like <Cat> contain other tags inside them, like <firstName>. This format is good for organizing the layout of a document in a tree-like format, just like HTML, where we want to nest elements like a sentence within a paragraph, for example. XML does not carry any information about how to be displayed and can be used in a variety of presentation scenarios

**XML**

```xml
<Cats> 
    <Cat> 
        <firstName>Smally</firstName> 
        <lastName>McTiny</lastName> 
    </Cat> 
    <Cat> 
        <firstName>Kitty</firstName> 
        <lastName>Kitty</lastName> 
    </Cat> 
    <Cat> 
        <firstName>Foots</firstName> 
        <lastName>Smith</lastName> 
    </Cat> 
    <Cat> 
        <firstName>Tiger</firstName> 
        <lastName>Jaws</lastName> 
    </Cat> 
</Cats> 
```

![Screenshot of XML cats file](/images/cats_XML.png)
This file is opened viewed on my Firefox browser from my local directory (right click on the file and choose to open in Firefox). You can also [download the XML file](https://github.com/DHRI-Curriculum/data-literacies/blob/v2.0-di-edits/files/cats.xml) if you would like to see what it looks like in other viewers. 

- - - 

JSON: Or JavaScript Object Notation, also uses a nesting structure, but with the addition of "key/value" pairs, like the firstName key which is tied to the Smally value (at least for the first cat!). JSON is popular with web applications that save and send data from your browser to web servers, because it uses the main language of web browsers, JavaScript, to work with data.

**JSON**

```json
{
    "Cats": [ 
        {
            "firstName": "Smally",
            "lastName": "McTiny"
        }, 
        {
            "firstName": "Kitty",
            "lastName": "Kitty"
        },
        {
            "firstName": "Foots",
            "lastName":"Smith"
        }, 
        {
            "firstName": "Tiger",
            "lastName":"Jaws"
        } 
    ]
} 
```

![Screenshot of JSON cats file](/images/cats_JSON.png)
This file is opened viewed on my Firefox browser from my local directory (drag and drop the file onto a open tab/window). You can also [download the JSON file](https://github.com/DHRI-Curriculum/data-literacies/blob/v2.0-di-edits/files/cats.json) if you would like to see what it looks like in other viewers. 

- - -

CSV: Or Comma Separated Values uses---you guessed it!---commas to separate values. Each line (First Name, Last Name) is a new "record" and each column (separated by a comma) is a new "field." This data format stores tabular data it a clean way that facilitates the transfer of data between different data architectures. As data types go, it is very rudimentary (even predating computers!) and is easy to type, without needing special characters beyond a comma.

**CSV**

```
First Name,Last Name
Smally,McTiny
Kitty,Kitty
Foots,Smith
Tiger,Jaws
```

![Screenshot of CSV cats file](/images/cats_CSV.png)
This file is opened viewed on my Firefox browser from my local directory (drag and drop the file onto a open tab/window). You can also [download the CSV file](https://github.com/DHRI-Curriculum/data-literacies/tree/v2.0-di-edits/files) (right click on `cats.csv` and click `save link as` to download the file to your local computer) if you would like to see what it looks like in other viewers. 


### The importance of using open data formats

A small detour to discuss data formats. For accessibility, future-proofing, and preservation, keep your data in open, sustainable formats. A demonstration:

1. Open [this file](https://raw.githubusercontent.com/DHRI-Curriculum/data-literacies/v2.0-di-edits/files/cats.csv) in a [text editor](https://github.com/DHRI-Curriculum/command-line/blob/v2.0-smorello-edits/sections/13-text-editors-ides.md) (e.g. VS Code, TextEdit (MacOs), NotePad (Windows) ), and then in an app like Excel. This is a CSV, an open, text-only, file format.
2. Now do the same with [this Excel file](https://github.com/DHRI-Curriculum/data-literacies/blob/v2.0-di-edits/files/cats.xlsx). Unlike the previous, this is a proprietary format! 

Sustainable formats are generally unencrypted, uncompressed, and follow an open standard.

<table>
    <caption>A small list of open formats:<sup>1</sup></caption>
    <tr>
        <th>Types of multimedia</th>
        <th>Examples</th>
         <th>Common file extensions</th>
    </tr>
    <tr>
        <th rowspan="3">Images</th>
         <td><a href="https://www.lifewire.com/tif-tiff-file-2622393">TIFF</a> (Tagged Image File Format) </td>
         <td>.tiff</td>
    </tr>
        <tr>
        <td><a href="https://en.wikipedia.org/wiki/JPEG_2000">JPEG2000</a></td>
        <td>.jp2, .jpf, .jpx</td>
    </tr>
    </tr>
        <tr>
        <td><a href="http://www.libpng.org/pub/png/pngintro.html">PNG</a> (Portable Network Graphics)</td>
        <td>.png</td>
    </tr>
        <tr>
        <th rowspan="3">Text</th>
         <td><a href="https://help.ceda.ac.uk/article/4429-ascii-formats">ASCII</a>  (American Standard Code for Information Interchange)</td>
         <td>.ascii, .dat, .txt</td>
    </tr>
        <tr>
        <td><a href="https://en.wikipedia.org/wiki/PDF">PDF</a> (Portable Document Format)</td>
        <td>.pdf</td>
    </tr>
        <tr>
        <td><a href="https://en.wikipedia.org/wiki/Comma-separated_values">CSV</a> (Comma-Seperated Values</td>
        <td>.csv</td>
    </tr>
    </tr>
        <tr>
        <th rowspan="2">Audio</th>
         <td><a href="https://xiph.org/flac/index.html">FLAC</a> (Free Lossless Audio Codec)</td>
         <td>.flac</td>
    </tr>
        <tr>
        <td><a href="https://xiph.org/ogg/">ogg</a></td>
        <td>.ogg</td>
    </tr>
    </tr>
        <tr>
        <th rowspan="2">Video</th>
         <td><a href="https://www.lifewire.com/mp4-file-2622024">MPEG-4</a></td>
         <td>.mp4</td>
    </tr>
        <tr>
        <td><a href="https://xiph.org/ogg/">ogg</a></td>
        <td>.ogg</td>
    </tr>
    </tr>
        <tr>
        <th rowspan="3">Others</th>
         <td><a href="https://www.w3schools.com/xml/xml_whatis.asp">XML</a> (Extensible Markup Language)</td>
         <td>.xml</td>
    </tr>
        <tr>
        <td><a href="https://www.json.org/json-en.html">JSON</a> (JavaScript Object Notation</td>
        <td>.json</td>
    </tr>
        <tr>
        <td><a href="https://www.3dsystems.com/quickparts/learning-center/what-is-stl-file">STL</a> (STereoLithography file format -- used in 3D modeling)</td>
        <td>.stl</td>
</table>

<sup>1</sup>More information on the file formats are linked in each example. For a list of file formats, consider the Library of Congress' list of <a href="https://www.loc.gov/preservation/digital/formats/fdd/browse_list.shtml#"> Sustainability of Digital Formats</a>.


### Challenge: Processed/Transformed

1. How do you decide the formats to store your data when you transition from 'raw' to 'processed/transformed' data? 
2. What are some of your considerations?

## Tidy Data

There are guidelines to the processing of data, sometimes referred to as **Tidy Data**.<sup>1</sup> One manifestation of these rules:

1. Each variable is in a column.
2. Each observation is a row.
3. Each value is a cell.

Look back at our example of cats to see how they may or may not follow those guidelines. **Important note**: some data formats allow for more than one dimension of data! How might that complicate the concept of **Tidy Data**?

```json
{
    "Cats": [
            {
                "Calico": [
                    {
                        "firstName": "Smally",
                        "lastName":"McTiny"
                    },
                    {
                        "firstName": "Kitty",
                        "lastName": "Kitty"
                    }
                ],
                "Tortoiseshell": [
                    {
                        "firstName": "Foots",
                        "lastName":"Smith"
                    },
                    {
                        "firstName": "Tiger",
                        "lastName":"Jaws"
                    }
                ]
            }
        ]
}
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
    
### Validity

Measurements must be valid, in that they must conform to set constraints:

1. The aforementioned "yes" or "y" or "1" should all be changed to one response.
2. Certain fields cannot be empty, or the whole observation must be thrown out.
3. Uniqueness, for instance no two people should have the same social security number.
    
### Accuracy

Measurements must be accurate, in that they must represent the correct values. While an observation may be valid, it might at the same time be inaccurate. 123 Fake street is a valid, inaccurate street address.

Unfortunately, accuracy is mostly acheived in the observation process. To be achieved in the cleaning process, an outside trusted source would have to be cross-referenced.

### Completeness

Measurements must be complete, in that they must represent everything that might be known. This also is nearly impossible to achieve in the cleaning process! For instance in a survey, it would be necessary to re-interview someone whose previous answer to a question was left blank. 
    
### Consistency

Measurements must be consistent, in that different observations must not contradict each other. For instance, one person cannot be represented as both dead and still alive in different observations. 
    
### Uniformity 

Measurements must be uniform, in that the same unit of measure must be used in all relevant measurements. If one person's height is listed in meters and another in feet, one measurement must be converted.

## Challenge: When do we stop cleaning?  

1. How do we know when our data is cleaned enough? 
2. What happens to the data that is removed? 
3. What are we choosing to say about our dataset as we prepare them for analysis?

## Analyzed

Analysis can take many forms (just like the rest of this stuff!), but many techniques fall within a couple of categories:

### Descriptive Analysis

Techniques geared towards summarizing a data set, such as:

- Mean
- Median
- Mode
- Average
- Standard deviation

### Inferential Analysis

Techniques geared towards testing a hypothesis about a population, based on your data set, such as:

- Extrapolation
- P-Value calculation

### Challenge: Analysis

1. As we consider the types of analysis that we choose to apply onto our data set, what are we representing and leaving out? 
2. How do we guide our decisions of interpretation with our choices of analyses? 
3. Are we comfortable with the intended use of our research? Are we comfortable with the unintended use of our research? What are potential misuses of our outputs? 
4. What can happen when we are trying to just go for the next big thing (tool/methods/algorithms) or just ran out of time and/or budget for our project?

## Visualized

Visualizing your data helps you tell a story and construct a narrative that guides your audience in understanding your interpretation of a collected, cleaned, and analyzed dataset. Depending on the type of analysis you ran, different kinds of visualization can be more effective than others. Below are some examples of data visualization that can help you convey the message of your data.

<table>
    <caption>Examples of Data Visualization</caption>
    <tr>
        <th>Types of Analysis</th>
        <th>Types of Visualization</th>
         <th>When to Use</th>
        <th>Example of Visualization</th>
    </tr>
    <tr height="300px">
        <th rowspan="3">Comparisons</th>
         <td>Bar charts</td>
         <td>Comparison across distinct categories</td>
        <td><img src="/images/D4PG_bar.png" alt="Bar Chart">From <a href="https://dataforgood.commons.gc.cuny.edu/report-on-covid-19s-impact-on-cuny-students/" target="_blank">The Data for Public Good</a> at the Graduate Center.</figcaption></td>
    </tr>
    <tr height="300px">
        <td>Histograms</td>
        <td>Comparison across continuous variable</td>
        <td><img src="/images/PolicyViz_histogram.png" alt="Histogram"><figcaption>From <a href="https://policyviz.com/2018/11/27/histogram-design-decisions/" target="_blank">Policy Viz.</figcaption></td>
    </tr>
    <tr height="300px">
        <td>Scatter plots</td>
        <td>Useful to check for correlation (not causation!)</td>
        <td><img src="/images/538_scatter.png" alt="Scatter plot"><figcaption>From <a href="https://fivethirtyeight.com/features/the-gops-primary-rules-might-doom-carson-and-cruz/" target="_blank">FiveThirtyEight.</figcaption></td>
    </tr>
    <tr height="300px">
        <th rowspan="3">Time</th>
        <td>Stacked area charts</td>
        <td>Evolution of value across different groups</td>
        <td><img src="/images/DatatoViz_stackedarea.png" alt="Stacked area chart"><figcaption>From <a href="https://www.data-to-viz.com/graph/stackedarea.html" target="_blank">From Data to Viz.</figcaption></td>
    </tr>
    <tr height="300px">
        <td>Sankey Diagrams</td>
        <td>Displaying flows of changes</td>
        <td><img src="/images/DatatoViz_sankey.png" alt="Sankey"><figcaption>From <a href="https://www.data-to-viz.com/graph/sankey.html" target="_blank">From Data to Viz.</figcaption></td>
    </tr>
   <tr height="300px">
        <td>Line graphs</td>
        <td>Tracking changes over time</td>
        <td><img src="/images/D4PG_line.jpg" alt="Line Graph"><figcaption>From <a href="https://dataforgood.commons.gc.cuny.edu/report-on-covid-19s-impact-on-cuny-students/" target="_blank">The Data for Public Good</a> at the Graduate Center.</figcaption></td>
    </tr>
    <tr height="300px">
        <th rowspan="2">Small numbers/percentages</th>
        <td>Pie charts</td>
        <td>Demonstrate proportions between categories</td>
        <td><img src="/images/DB_pie.jpg" alt="Pie chart"><figcaption>From <a href="https://www.loc.gov/pictures/search/?q=%22lot%2011931%22%20NOT%20medal&st=grid&co=anedub&loclr=blogpic" target="_blank">The Library of Congress.</figcaption></td>
    </tr>
    <tr height="300px">
        <td>Tree maps</td>
        <td>Demonstrate hierarchy and proportion</td>
        <td><img src="/images/DataViz_treemap.png" alt="Tree map"><figcaption>From <a href="https://datavizcatalogue.com/methods/treemap.html" target="_blank">The Data Visualization Catalogue.</figcaption></td>
    </tr>
    <tr height="300px">
        <th rowspan="2">Survey responses</th>
        <td>Stacked bar charts</td>
        <td>Compares total amount across each group (e.g. plotting Likert scale)</td>
        <td><img src="/images/DB_stackedbar.jpg" alt="Stacked bar charts"><figcaption>From <a href="https://www.loc.gov/pictures/search/?q=%22lot%2011931%22%20NOT%20medal&st=grid&co=anedub&loclr=blogpic" target="_blank">The Library of Congress.</figcaption></td>
    </tr>
    <tr height="300px">
        <td>Nested area graphs</td>
        <td>Visualize branching/nested questions</td>
        <td><img src="/images/evergreen_nestedarea.jpg" alt="Nested area graph"><figcaption>From <a href="https://stephanieevergreen.com/nested-area-graph/" target="_blank">Evergreen Data.</figcaption></td>
    </tr>
    <tr height="300px">
        <th rowspan="2">Place</th>
        <td>Choropleth maps</td>
        <td>Visualize values over a geographic area to demonstrate pattern</td>
        <td><img src="/images/DB_choropleth.jpg" alt="Choropleth map"><figcaption>From <a href="https://www.loc.gov/pictures/search/?q=%22lot%2011931%22%20NOT%20medal&st=grid&co=anedub&loclr=blogpic" target="_blank">The Library of Congress.</figcaption></td>
    </tr>
    <tr height="300px">
        <td>Hex(bin) or Tile maps</td>
        <td>Similar to Choropleth with the hexbin/tile representing regions equally rather than by geographic size</td>
        <td><img src="/images/rgraph_hexbin.png" alt="Hexbin graph"><figcaption>From <a href="https://www.r-graph-gallery.com/328-hexbin-map-of-the-usa.html" target="_blank">R Graph Gallery.</figcaption></td>
    </tr>
    <tr>
        <th colspan="4"> Adapted from <a href="https://us.sagepub.com/en-us/nam/effective-data-visualization/book265203_"> Stephanie D. Evergreen (2019) Effective data visualization : The right chart for the right data</a>, <a href="https://datavizcatalogue.com/">The Data Visualisation Catalogue</a>, and <a href="https://www.data-to-viz.com/">From Data to Viz</a></th>
    <tr>
</table>

This table is a teaser for the many possibilities of what data visualization can be. Creating a visual for your data is an art form and you can sometimes find yourself spending a significant amount of time looking for the best ways to visualize your data.

An example of effective data visualization can be seen in W.E.B. Du Bois [data potraits at the Paris Exposition in 1900](https://www.loc.gov/pictures/search/?q=%22lot%2011931%22%20NOT%20medal&st=grid&co=anedub&loclr=blogpic), as part of [the Exhibit of American Negroes](https://en.wikipedia.org/wiki/The_Exhibit_of_American_Negroes_). Using engaging hand-drawn visualizations, he tells the narrative of what it meant to be Black in post-Emancipation America as he translates sociological research and census data to reach beyond the academy. Head [here](https://hyperallergic.com/476334/how-w-e-b-du-bois-meticulously-visualized-20th-century-black-america/) to read more about Du Bois' project. 

### Challenge: Visualizations

As we transform our results into visuals, we are also trying to tell a narrative about the data we collected. Data visualization can help us to decode information and share quickly and simply.

1. What are we assuming when we choose to visually represent data in particular ways? 
2. As you may have realized, many of the visualization examples work with quantitative data, as such, how do you think we can visualize qualitative data? (e.g. Word Clouds, Heat Map)
3. How can data visualization mislead us? (for e.g. [Nathan Yau discusses how data visualization can lie](https://flowingdata.com/2017/02/09/how-to-spot-visualization-lies/)
4. How can data visualization help us tell a story? (for e.g. [Data Feminism's On rational, Scientific, Objective Viewpoints from Mythical, Imaginary, Impossible Standpoints](https://mitpressonpubpub.mitpress.mit.edu/pub/8tjbs2x5/release/2))



# Data Literacy and Ethics

Throughout the workshop we have been thinking together through some of the potential ethical concerns that might crop up as we proceed with our own projects. Just as we have disucssed thus far, we hope that you see that data and ethics is an ongoing process throughout the lifespans of your project(s) and don’t often come with easy answers.

## Activity

In this final activity, we would like for you to think about some of the potential concerns that might come up in the scenario below and discuss how you might approach them:

You are interested in looking at the reactions to the democratic party presidential debates across time. You decided that you would use data from twitter to analyze the responses. After collecting your data, you learned that your data has information from users who were later banned and included some tweets that were removed/deleted from the site.

### If you would like some guiding questions:

- What are some reasons you might have for anonymizing (or not) your data? 
    - Would your approach differ if the responses were anonymized v. not?
- Would you remove the data in your initially downloaded corpus?
    - How might you be aware of the differences in the corpus you downloaded v. the most current information?
- Would the number of tweets generated impact your decisions?
- How might where you are at in your project (e.g. "raw" data v. "cleaned" data v. analysed) affect your choices?

### Some additional exploration:

- If you were collecting and/or analyzing data on folx in power, such as looking at the data from [Tweets of Congress's](https://alexlitel.github.io/congresstweets/) project, wouuld that change the way you consider your answers to the previous questions?
- Current [ethical guidelines](https://safelab.socialwork.columbia.edu/content/ethics) from SAFE Lab at Columbia University have decided to alter the text of social media post to render it unsearchable. Why and when would you consider (or not) altering the collected tweets for publication? 

# Some concluding thoughts

Data and ethics are contextually driven. As such, there isn’t always a risk-free approach. We often have to work through ethical dilemmas while thinking through information that we may not have (what are the risks of doing/not doing this work?). We have approached a moment where the question is no longer what we could do but what we should do. Given this saturated data-driven world we currently live in, there is value is pausing and consider why and what we are collecting, researching, analyzing, and understanding. Starting on a new project, especially one dealing with "big" data can be exciting but we now also have to first consider who does the data collected benefit and why is it important are important.

For a set of great questions to help you think through your data exploration and project planning, please check out Kristen Hackett's Tagging the Tower post, *[What to Consider when Planning a Digital Project.](https://digitalfellows.commons.gc.cuny.edu/2019/10/30/what-to-consider-when-planning-a-digital-project/)*
