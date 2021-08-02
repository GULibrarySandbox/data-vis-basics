---
title: RAWGraphs
nav: true
---

# RAWGraphs.io

-----

RAWGraphs [https://rawgraphs.io/](https://rawgraphs.io/) is an open source (free) online tool to create publication quality visualisations from complex tabular data.  The platform was developed at the [Density Design Research Lab](http://www.densitydesign.org) of the Politecnico di Milano.

The RAWGraphs tool allows users to easily and quickly create data visualisations.  These visualisations can be exported and edited in an image editing tool (such as Adobe Photshop, or open source free tool GIMP), embedded in a webpage or imported into a document.  

Features and chart options include:

- Scatter Plots
- Area Graphs
- Alluvial Diagrams
- Circular & Cluster Dendograms
- Contour plots and more...

{% include figure.html img="RawGraphsTypes.png" alt="RawGraphs chart types" caption="RawGraphs chart types" width="100%" %}![image](https://user-images.githubusercontent.com/51395844/127804546-7c56722d-976b-4911-b5bc-008ce8774792.png)
Source: https://app.rawgraphs.io/ 

RAWGraphs is an online tool so don’t use personal, confidential or sensitive data.  However, should you need to visualise sensitive data, you can run an instance of RAWGraphs locally on your machine with [git](http://git-scm.com/book/en/Getting-Started-Installing-Git) and [Bower](http://bower.io/#installing-bower) software.

{% capture alert %}Cite the tool's developers when publishing a visualisation created using Voyant Tools: 

Mauri, M., Elli, T., Caviglia, G., Uboldi, G., & Azzi, M. (2017). *RAWGraphs: A Visualisation Platform to Create Open Outputs. In Proceedings of the 12th Biannual Conference on Italian SIGCHI Chapter.* New York, NY, USA: ACM. https://doi.org/10.1145/3125571.3125585 {% endcapture %} {% include alert.md text=alert color="warning" %}


## How to use RAWGraphs

Watch this video, using RAWGraphs sample data, to learn how to create a Violin Plot.

Topics covered:
- Upload a dataset to RAWGraphs.io (00:03)
- Preview and check the data  (00:30)
- Choose the most appropriate chart (01:55)
- Violin Plot description  (02:17)
- Map dataset variable to chart dimensions (02:46)
- Customise the chart (03:23)
- Export the chart image file (05:28)

<iframe src="https://player.vimeo.com/video/558349816" width="640" height="564" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe>

Practice creating visualistions by doing Activities 1 and 2 below.

### Activity 1: Create an Alluvial diagram

**About the data

The sample dataset to work with is from Griffith University's Prosecution Project, cited as:

Finnane, Mark, 2019, "Queensland Supreme Court Trials 1850-1899",
doi:10.26193/6YOCXO, ADA Dataverse, V1, UNF:6:cB3aNxfy6JBMKg8tHM/W1g==  [https://
dataverse.ada.edu.au/dataverse/australian_historical_criminal_justice_data?q=queensland](https://
dataverse.ada.edu.au/dataverse/australian_historical_criminal_justice_data?q=queensland)

The original dataset presents 40 years of criminal trials from 1850-1899, their location, type of conviction, sentence, sex and other variables, with over 10,000 observations.

Some variables have been aggregated to create categorical data, several variables and values have been removed and values cleaned for the purposes of training.  This data preparation was undertaken in [OpenRefine](https://openrefine.org/).

The resulting sample dataset has 976 observations and eight variables including an ID,defendant's sex, offence, place of trial, trial judge’s name, verdict, trial year and sentence given.

**Watch this video demonstrating the steps in Activity 1.

Topics covered:
- Step 1: upload the dataset to RAWGraphs.io (00:07)
- Preview and check the data  (00:25)
- Step 2: select an Alluvial diagram (00:38)
- Step 3: map data to the variables  (00:50)
- Preview the results (01:25)
- Add one more variable (02:35)
- Step 4: customise the chart (03:38)
- Step 5: export the chart image file (05:09)
- Extra steps (5:30)

<iframe src="https://player.vimeo.com/video/560748075" width="640" height="564" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe>

{% capture text %}
{% endcapture %} {% include card.md header="Step 1: upload the data" text=text %}

{% capture text %}
Use the strategy above to remove the right-hand bracket (")") from the  `Suburb_PostCode`  column.
- `value.replace(")", "")`{% endcapture %} {% include card.md header="Activity - remove another character" text=text %}

It is easy to re-use GREL expressions, as OpenRefine provides a history of commands. You can select them and reuse as is or make changes. Let's try this with the remainder of the unnecessary characters in the  `Suburb_PostCode`  column. You want only to have a separator left between our two values in each cell.  The comma is the separator in this variable.

{% capture text %}
- at  `Suburb_PostCode` column, select  `Edit cells > Transform ...`
- click the  `History`  tab
- click on the first  `Reuse`  option
- click inside the expression box, change character  `")",""` to `", ",","`  (i.e. comma & space character to comma no space character)
- preview to check correctness
- click  `OK`.{% endcapture %} {% include card.md header="Activity - repeat transformation steps by using History" text=text %}

{% include button.md text="See the steps taken in this video" link="https://vimeo.com/412605118/b259dd9e3c" color="info" %}

-----

Let's explore the  `Suburb_PostCode`  column to see which postcodes were the most or least prominent traffic crash locations.

### Splitting cells

Splitting multi-valued cells will enable faceting by text. This is also useful for splitting full names in first and last name columns and more.

{% capture text %}
- Click down arrow at the top of the  `Suburb_PostCode`  column.
- Choose  `Edit cells > Split multi-valued cells`
- At the separator Expression box, check that the correct separator, i.e. a comma, is specified.
- Click  `OK`.

Note that the rows are still numbered sequentially and that there are now 55056 rows, which no longer reflects one row per accident record. These are compound data objects.

- Click the  `Records`  option to change to  `Records`  mode and then go back to  `Rows`.

Note how the numbering changes as you toggle – indicating that several rows are related to the same record. This method is useful for  `JSON`  and  `xml`  files which have compound data objects.

It would be possible to use a text facet to see this data, but this is not the most efficient method.{% endcapture %} {% include card.md header="Activity - splitting cells" text=text %}

-----

### Undo and Redo

It is common while exploring and cleaning a dataset to discover after you've made a change that you really should have done something else first. OpenRefine provides *Undo* and *Redo* operations to make this easy, no matter how far along you have gone.

{% capture text %}
- Click where it says  `Undo / Redo`  on the top left side of the screen. All the changes you have made so far are listed here.
- Click on the previous step, to remove the split in the cell values of  `Suburb_PostCode`  column.
- Visually confirm that the columns data has been re-joined.

Go back a step
- before moving on to the next lesson,  `Undo`  to the step **before** we first used GREL to remove all the extra characters in  `Suburb_PostCode`.
- Go back to  `Facet/filter tab`.{% endcapture %} {% include card.md header="Activity - Undo" text=text %}

-----

### Join up GREL commands

Let's perform the earlier clean up steps and customised text faceting for  `Suburb_PostCode`  column. We can do this more efficiently by joining up the GREL expressions.

{% capture text %}
- select  `Suburb_PostCode`  column.  All three cleaning steps can be performed by combining  `value.replace`  expressions.
- select  `Edit cells > Transform ...`
- in the Expression box, enter  `value.replace("(", "").replace(")", "").replace(", ", ",")`
- *Preview* the changes
- click `OK`{% endcapture %} {% include card.md header="Activity - join up GREL commands" text=text %}

-----

### Split multi value cells into multiple columns (tidy data)

Let's split  `Suburb_PostCode`  data into two columns one for suburb and another for postcode.

{% capture text %}
- select  `Suburb_PostCode`  column
- select `Edit Column > Split into several columns` ...
- keep the Separator as a comma, and split the data into two columns
- leave the *After Splitting* boxes checked
- Click  `OK`.

The original column has now been replaced with two columns for different values.

A column named  `Suburb_PostCode 1`  contains the names of suburbs.

A column named  `Suburb_PostCode 2`  contains postcodes in green characters.  

The change in colour denotes that OpenRefine has changed the underlying *format* of the data from *text* to *number*.

Let's edit the column headings to represent the data more accurately.

- go to  `Suburb_PostCode 1`
- select  `Edit Column > Rename this column`  and enter  `Suburb`  as the new column name
- repeat the process for  `Suburb_PostCode 2`  to rename the column to  `Postcode` .{% endcapture %} {% include card.md header="Activity - joining up GREL commands" text=text %}


{% include button.md text="Watch this video for instructions" link="https://vimeo.com/412605933/d8be2a9d15" color="info" %}


-----

<p align="center">
  <a href="https://griffithunilibrary.github.io/data-vis-basics/content/5-voyant.html"><-- BACK</a> |
  <a href="https://griffithunilibrary.github.io/data-vis-basics/content/7-more.html">NEXT --></a>
</p>
