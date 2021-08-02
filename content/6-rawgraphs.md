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

{% include figure.html img="RawGraphsTypes.png" alt="RawGraphs chart types" caption="RawGraphs chart types" width="100%" %}
Source: [https://app.rawgraphs.io/](https://app.rawgraphs.io/)

RAWGraphs is an online tool so don’t use personal, confidential or sensitive data.  However, should you need to visualise sensitive data, you can run an instance of RAWGraphs locally on your machine with [git](http://git-scm.com/book/en/Getting-Started-Installing-Git) and [Bower](http://bower.io/#installing-bower) software.

{% capture alert %}Cite the tool's developers when publishing a visualisation created using Voyant Tools: 

Mauri, M., Elli, T., Caviglia, G., Uboldi, G., & Azzi, M. (2017). *RAWGraphs: A Visualisation Platform to Create Open Outputs. In Proceedings of the 12th Biannual Conference on Italian SIGCHI Chapter.* New York, NY, USA: ACM. https://doi.org/10.1145/3125571.3125585 {% endcapture %} {% include alert.md text=alert color="warning" %}


## How to use RAWGraphs

Watch this video, using RAWGraphs sample data, to learn how to create a Violin Plot.  Then practice creating visualistions by doing Activities 1 and 2 below.

Topics covered:
- Upload a dataset to RAWGraphs.io (00:03)
- Preview and check the data  (00:30)
- Choose the most appropriate chart (01:55)
- Violin Plot description  (02:17)
- Map dataset variable to chart dimensions (02:46)
- Customise the chart (03:23)
- Export the chart image file (05:28)
<iframe src="https://player.vimeo.com/video/558349816" width="640" height="564" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe>
### Activity 1: Create an Alluvial diagram

**About the data**

The sample dataset to work with is from Griffith University's Prosecution Project, cited as:

Finnane, Mark, 2019, "Queensland Supreme Court Trials 1850-1899",
doi:10.26193/6YOCXO, ADA Dataverse, V1, UNF:6:cB3aNxfy6JBMKg8tHM/W1g==  [https://
dataverse.ada.edu.au/dataverse/australian_historical_criminal_justice_data?q=queensland](https://
dataverse.ada.edu.au/dataverse/australian_historical_criminal_justice_data?q=queensland)

The original dataset presents 40 years of criminal trials from 1850-1899, their location, type of conviction, sentence, sex and other variables, with over 10,000 observations.

Some variables have been aggregated to create categorical data, several variables and values have been removed and values cleaned for the purposes of training.  This data preparation was undertaken in [OpenRefine](https://openrefine.org/).

The resulting sample dataset has 976 observations and eight variables including an ID,defendant's sex, offence, place of trial, trial judge’s name, verdict, trial year and sentence given.

**Watch this video demonstrating the steps in Activity 1**

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
- Go to Griffith’s Research Data Storage Service [here](https://research-storage.griffith.edu.au/owncloud/index.php/s/W7laRdfRXgp4504)
- Download `2021_QLD_Supreme_Court_Trials_1850-1899_Subset4.csv`
- Save file
- Go to [https://rawgraphs.io/](https://rawgraphs.io/) and click `use it now`.
- Select `Upload` > `Browse` > go to `Downloads folder` > click on dataset > `Open`
- It might take a few seconds to upload, with 976 rows parsed.
{% endcapture %} {% include card.md header="Step 1: upload the data" text=text %}

{% capture text %}
Alluvial diagrams represent flows to see correlations between categorical dimensions, visually linking to the number of elements sharing the same categories.
- Click on `Alluvial Chart` box
{% endcapture %} {% include card.md header="Step 2: select Alluvial chart" text=text %}

{% capture text %}
The variables are listed in the green boxes.  Firstly create a chart to identify any patterns between Offences, Verdicts and Sentencing.
- Scroll down to `Map dimensions`
- Add two variables to the `Steps dimension`, drag and drop in this order
  - `Offence`
  - `Verdict`
- Size dimension isn't used in this tutorial.
{% endcapture %} {% include card.md header="Step 3: map the variables to the chart" text=text %}

{% capture text %}
The black vertical lines are called bars or nodes and represent the values within the variables.

The first step is `Offence`, with seven nodes, one for each type of Offence.  The size of the seven nodes (Offence types in this dataset) is proportional to the number of values within the node or in this case, the number of offences heard by type.

The second step is `Verdict`, and it’s composed of five nodes (or value options), representing the different Verdict types.  Again, the size of each node is proportional to the number of rows in the dataset containing that specific value.

The same logic applies to any additional steps.
- `Scroll` back up to `Mapping dimensions`
- Drag and drop `Sentence` into the `Steps dimension` box
- Scroll down to preview to see thirteen nodes, categorising the types of `Sentence` ordered by the judge.

The flows between nodes in the two steps represent the number of lines in the dataset sharing the same couple of values: for example, the largest flow is from the Larceny node in the Offence step and the Guilty node in the Verdict step, and the largest proportion of this group flows to 12-18 months hard labour node.

We can see easily, by the flow of the nodes and the colours, the proportion of offences, the proportion of verdict types and sentence ranges, in a very simple visual for a dataset of almost 1000 observations.

When publishing, the data should accompany the article to verify the visualisation.{% endcapture %} {% include card.md header="Preview the results" text=text %}

{% capture text %}
Customise the visualisation using the up/down arrows to make changes to:

`Artboard`:
- `Width`:  1000
- `All margins`: 30

`Chart`:
- `Nodes width`: 5
- `Padding`: 25
- `Links opacity`: .5
- `Sort nodes by`: size (descending)
- `Flows alignment`: Center

`Colours`:
- Click on `colour schemes` to choose one of three default options
or 
- click on each of the `variables' colours` to see palettes, then click within the colour palette box to make changes
or 
- paste a  `#Hex code` for a colour of your choice such as #fb082f
- Explore results
- 
`Labels`:
 - Select `Yes` to show values. It looks a bit busy, let’s `turn them off`. You can include more details on the data in a publication text and appendix.

*Note for MAC Users*: Some options are slightly different. If you want to change a specific thing such as axis line thickness, you have to click on it first as there won’t be an option to select which axis you are working on in the formatting pane.{% endcapture %} {% include card.md header="Step 4: Customise results" text=text %}

{% capture text %}
- Name the chart according to a file name convention required by the publisher or your data management protocols.
- Change the file type according to publisher requirements, `.jpg` will provide the highest quality file from this tool.
- Select download

To make further changes to the chart, use a image editor tool such as those demonstrated in [Create a publication quality image](https://griffithunilibrary.github.io/data-vis-basics/content/4-convert.html) activities. 
{% endcapture %} {% include card.md header="Step 5. Export" text=text %}

{% capture text %}
Play further with the variables to explore the dataset.
- Scroll back to `Step 3: Mapping`
- Click `x` on the green boxes in `Steps`
- Drag and drop `Def_sex` (sex of defendant) and `Offence` and explore in `Step 4` to
- visualise sex differences in the types and proportions of offences.
- Scroll back to `Step 3: Mapping`
- Exchange the variables for `Trial Judge` as `Step 1` and `Trial Place` as `Step 2`, to explore which judges worked across different locations in Queensland.{% endcapture %} {% include card.md header="Extra" text=text %}

{% include figure.html img="2021_Offences_Fig_V1.jpg" alt="RAWGraphs Alluvial Chart of a Prosecution Project dataset" caption="RAWGraphs Alluvial Chart of a Prosecution Project dataset" width="100%" %}

Lesson adapted from:

"How to make an alluvial diagram", by RAWGraphs Team. Licensed under CC BY-NC-SA4.0. Accessed: February 12, 2020, from [https://rawgraphs.io/learning/how-to-make-an-
alluvial-diagram/](https://rawgraphs.io/learning/how-to-make-an-alluvial-diagram/) 

### Activity 2: time series data visualisation

**About the data**

The sample dataset in this tutorial features Brisbane’s daily maximum temperatures in 2019, and is from the Australian Bureau of Meteorology’s (BOM) Climate Data series: [http://www.bom.gov.au/climate/data/](http://www.bom.gov.au/climate/data/).

You can choose a range of years from BOM data, in this instance one full year has been used. BOM has excellent visualisation tools for use on its website including here which shows the range of daily maximum temperatures quite clearly.

In this activity you will visualise the most prevalent maximum daily temperatures across 2019, using the `Contour plot` in RAWGraphs.

{% capture text %}
- Go to Griffith’s Research Data Storage Service link [here](https://research-storage.griffith.edu.au/owncloud/index.php/s/OFbexAoD0u1dIFH) 
- Download the sample dataset `2019_BOM_Brisbane_MaxTempData_V2.csv`
- `Save` file
- Go to [https://rawgraphs.io/](https://rawgraphs.io/) and click `use it now`
- Select `Upload` > `Browse` > go to `Downloads` folder > click on dataset `2019_BOM_Brisbane_MaxTempData_V2.csv`> `Open`
- Preview the data to ensure 365 rows have been parsed.{% endcapture %} {% include card.md header="Step 1: upload the data" text=text %}

{% capture text %}
A Contour plot shows the estimated density of point clouds, which is especially useful to avoid overplotting in large datasets.
- Click on `Contour plot` box
- Scroll down to `Step 3`
{% endcapture %} {% include card.md header="Step 2: choose a Contour plot" text=text %}

{% capture text %}
The variables are listed in the green boxes.  Let’s create a chart to show if there are particular dates with a large proportion of maximum temperatures throughout the year 2019.
- Drag and drop `Date` variable to `X Axis` box
- Drag and drop `Max Temp` to `Y Axis` box
{% endcapture %} {% include card.md header="Step 3: Map the variables to the chart" text=text %}

{% capture text %}
Make changes to:

Artboard:
- `Width`:  940 px (pixels)
- `Height`: 483 px

Chart:
- `Show dots`: Yes

Colours: to change to greyscale
- `Color scale`: Sequential
- `Start colour`: click on `# Hex value` and paste `#E4E7EC` into the Hex Box 
or
- Click inside the `palette box` for an appropriate light grey shade, then click out of box
- `End colour`: click on `# Hex value` and paste `#181919` into the Hex Box
or
- Click inside the `palette box` for an appropriate dark grey shade, then click out of box

Labels:
- No need to show labels, but you can play with this to see the difference.

It is now quite easy to see the maximum temperatures which were most prevalent at different times of the year, with some darker clusters in mid-January to early February, and from mid-April to early May.  You can turn off the data points and just see the clusters, however it then doesn’t show the individual temperatures.
{% endcapture %} {% include card.md header="Step 4: Customise the chart" text=text %}

{% capture text %}
- Name the chart according to a file name convention required by the publisher or your data management protocols.
- Change the file type according to publisher requirements, `.jpg` will provide the highest quality file from this tool.
- Select download

To make further changes to the chart, use a image editor tool such as those demonstrated in [Create a publication quality image](https://griffithunilibrary.github.io/data-vis-basics/content/4-convert.html) activities. 
{% endcapture %} {% include card.md header="Step 5. Export" text=text %}

-----

<p align="center">
  <a href="https://griffithunilibrary.github.io/data-vis-basics/content/5-voyant.html"><-- BACK</a> |
  <a href="https://griffithunilibrary.github.io/data-vis-basics/content/7-more.html">NEXT --></a>
</p>
