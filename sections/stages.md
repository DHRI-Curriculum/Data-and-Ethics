[<<< Previous](forms.md) | [Next >>>](cleaned.md)

# Stages of Data

We begin without data. Then it is observed, or made, or imagined, or generated. After that, it goes through further transformations:

## Raw
    
Raw data is yet to be processed, meaning it has yet to be manipulated by a human or computer. Received or collected data could be in any number of formats, locations, etc.. It could be in any of the forms listed above.

But "raw data" is a relative term, inasmuch as when one person finishes processing data and presents it as a finished product, another person may take that product and work on it further, and for them that data is "raw data".

## Processed/Transformed

Processing data puts it into a state more readily available to analysis. For instance it could be rendered as **structured data**, i.e., in a table. This can also take many forms. Here are a few you're likely to come across, all representing the same data:

### XML

```
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

### JSON

```
{"Cats":[ 
    { "firstName":"Smally", "lastName":"McTiny" }, 
    { "firstName":"Kitty", "lastName":"Kitty" }, 
    { "firstName":"Foots", "lastName":"Smith" }, 
    { "firstName":"Tiger", "lastName":"Jaws" } 
]} 
```

### CSV
```
First Name,Last Name/n
Smally,McTiny/n
Kitty,Kitty/n
Foots,Smith/n
Tiger,Jaws/n
```
#### The importance of using open data formats
A small detour to discuss (the ethics of?) data formats. For accessibility, future-proofing, and preservation, keep your data in open, sustainable formats. A demonstration:

1. Open [this file](cats.csv) in a text editor, and then in an app like Excel. This is a CSV, an open, text-only, file format.
2. Now do the same with [this one](cats.xlsx). This is a proprietary format! 

Sustainable formats are generally unencrypted, uncompressed, and follow an open standard. A small list:

ASCII

PDF 

.csv

FLAC

TIFF

JPEG2000

MPEG-4

XML

RDF

.txt

.r



[<<< Previous](forms.md) | [Next >>>](cleaned.md)
