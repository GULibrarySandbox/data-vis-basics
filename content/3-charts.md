---
title: Charts
nav: true
---

Data visualisation using Microsoft Excel Part two: Charts

You don’t need a PivotTable to create a chart – charts can be created from any raw data – but, as per the previous exercises, your writing will generally deal with one aspect of the data at a time, so the figures created for inclusion in each section should represent that single discussion. 

{% text capture %}
1.	Select cells `K10:P12`.
2.	Click the `Insert` tab on the ribbon.
3.	Click `Column or Bar Chart`.  Choose `2-D column`.
4.	The chart is referred to as a `PivotChart` because it is based on a PivotTable.{% endcapture %} 
{% include card.md header="Activity : Creating a chart" text=text %}

{% include figure.html img="2021_Excel-data-visualisation_Student-workbook.jpg " alt="PivotChart" caption="PivotChart" width="100%" %}

## Rules for publication-quality visulatisations

As you have seen, Excel produces an aesthetically pleasing chart that is formatted according to the Theme of your workbook, but there are specific rules used to create publication-quality visuals which means some editing of your chart.

- No title required (will be captioned)
- Remove the Excel field buttons
- Remove the gap between the columns in a column chart
- No Colour – Black/White/Grey
- Legend top right
- Enhance the horizontal axis bar settings
- Match the vertical axis bar settings to the horizontal axis bar and add tick marks
- No background gridlines
- Include error bars (if applicable)
- Add an asterisk directly above the significant error bar (if applicable)
- Add axis titles
- Use large clear fonts for all text areas
- No border

### Chart tools

The following sections describe how to prepare your chart for publication. 

#### Tool: PivotChart Tools tab

- Navigate through records using *previous/next/first/last* navigation options at the top right of the table of data
- Use the drop-down menus at the top of each column to work with data
- Selecting an option in a particular column (e.g., to make a change to the data), affects all the cells in that column 
- Perform changes one column at a time, even when making changes across several columns 


###  Rows and Records

OpenRefine has two modes of viewing data: 'Rows' and 'Records'. 
- Rows mode: each row represents a single record in the data set
- Records mode, OpenRefine can link together multiple rows as belonging to the same record 

This is useful when working with `xml` files, MARC records, as well as `csv` files. We will see an example of this later.

{% include figure.html img="ORLayout.png" alt="OpenRefine layout" caption="OpenRefine layout" width="75%" %}

### Undo / Redo

OpenRefine provides Undo and Redo operations to make changes to your data work, going back to your very first action. Find out how this works in the [GREL](https://griffithunilibrary.github.io/intro-data-wrangle/content/6-lesson.html) activities. 

### Saving projects

Projects are saved automatically as you work on them,  so there is no need to save copies as you go along. 

### Opening existing projects

To open an existing project in OpenRefine, click  `Open Project`  from the main OpenRefine screen (in the left-hand menu). 
When you click this, you will see a list of the existing projects and can click on a project's name to open it.

{% include button.md text="Watch this video to see OpenRefine's layout" link="https://vimeo.com/412542634/f5b1ced9b9" color="info" %}

-----

<p align="center">
  <a href="https://griffithunilibrary.github.io/intro-data-wrangle/content/2-tables.html"><-- BACK</a> |
  <a href="https://griffithunilibrary.github.io/intro-data-wrangle/content/4-lesson.html">NEXT --></a>
</p>
