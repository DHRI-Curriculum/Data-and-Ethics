← [Data is Foundational](01-data-is-foundational.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Stages of Data: Raw](03-stages-of-data-raw.md) →

---

# 2. Stages of Data

We begin without data. Then it is observed, or made, or imagined, or generated. After that, it goes through further transformations. Stages of data typically consist of a) collection of "raw" data, b) processing and/or transforming data, c) cleaning, d) analysis, and e) visualization. For example, we can consider the stages in the following way:

- We start with formulating a research question(s) or hypotheses and set up a project to answer our question(s).
    - E.g. What proportion of the artwork collected and/or hosted in the Met are by non cis-gender men artists and also in public domain?
- In the process of setting up the project, we make decisions on what kind of data we think can help us to answer the question
    - E.g. I think I can get the data from the Met's [open access data set](https://media.githubusercontent.com/media/metmuseum/openaccess/master/MetObjects.csv). I will need to look at what variables exist in the dataset to find out if I can filter by gender and the variables that will correspond to copyrights.
- After collecting our data we then consider and make decisions in the processes of cleaning.
    - E.g. I have to transform some of the gender values and decide what to do with the missing fields.
- We then run our preliminary analysis of the data.
    - E.g. I can run an analysis of the subset of non cis-gender men and public domain media objects against the total number of media objects to find out the proportion.
- At the end of our analysis, a decision is then made about how would we would present the data and its analysis.
    - E.g. I can present the result in a pie chart.

This is one cycle in which data goes from collection to transformation to visualization. This is also *not* the only way to go through the stages. For example, we could do a preliminary analysis first, such as running a correlation of variables, to explore what is missing before we begin the process of cleaning. Often, we also end up doing multiple iterations of cleaning and analysis, making decisions and choices to collapse particular variables or remove them entirely at each iterations. Making sure that we keep a clear documentation of our process will ensure that we are accountable to the data we have collected/are using and also ensure that our results can be replicated and reproduced if others choose to work on our "raw" data.

## Naming Conventions for Directory Structures

Before beginning your data collection, manipulation, and transformation, a good practice is to determine your file naming conventions. How many times have named something as `XXX_FinalFINALFINAL.pdf` or have difficulty searching for a version of the file that contained all that good idea that was edited out in the `XXX_FinalFINALFINALFINAL.pdf` version? While tools like version controlling with git can be helpful, we can also begin with setting up file naming conventions that can help us succeed! Here's an example from [Stanford](https://library.stanford.edu/research/data-management-services/case-studies/case-study-file-naming) that demonstrates the problems of badly name files in our projects.

For example, The Graduate Center's [Data Management](https://libguides.gc.cuny.edu/c.php?g=159618&p=1045090) guide suggest that top level folders (such as your main project folder) should include your project title, a unique identifier and the date (year) of your project (e.g. `dataliteracies_XYZ_2020`). Your sub folders and individual files should follow a similar system, with an identifiable activity or project in the file name (e.g. a sub-folder of the project: `sections_xyz_2020`, a file in the project: `lessons_XYZ_2020.doc`).

## Keywords

Do you remember the glossary terms from this section?

- [Data](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/data.md)

---

← [Data is Foundational](01-data-is-foundational.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Stages of Data: Raw](03-stages-of-data-raw.md) →