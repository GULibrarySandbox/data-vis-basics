---
title: Excel
nav: true
---

# Data visualisation using Microsoft Excel

{% include figure.html img="2021_Excel-data-visualisation_Student-workbook.jpg " alt="Data visualisation using Excel" caption="Data visualisation using Excel" width="100%" %}

### Overview

Undertake the activities below to create PivotTables and PivotCharts.

{% capture text %}
- MS Excel software 
- download activity .xls dataset from Griffith University's Research Data Storage [here](https://research-storage.griffith.edu.au/owncloud/index.php/s/7VHsCVyUsAKsTll){% endcapture %}
{% include card.md header="Setup" text=text %}

-----

### Data collection and use

The activity worksheet contains data about workshop attendances for 2019 and is broken down by Skill Group (column A), Trimester (column B) and across Academic Groups and Special Interest Groups (columns C to H).

Data is usually collected as a whole dataset, but generally analysed and used in “chunks”, particularly when writing up your findings. 

Let’s say Section 1 of a document compares and discusses attendance fluctuation in each academic group attendance across trimesters, while Section 2 discusses what type of session content (i.e. skill group) was in demand across the various academic groups.  Each section of the document should contain graphs that represent the data for the specific topic only. 

Even though this is a small dataset, it is quite difficult to analyse visually - imagine if this was a large dataset!

#### Data extraction
Let’s find out how many students from each academic group attended per trimester. 

{% capture text %}
1.	In the worksheet, click into cell `K1`.  Type `Attendance by Trimester`.
2.	Select cells `A2:H10`.  There’s no need to include any calculated totals in the selection as data can be calculated separately in the PivotTable.  Similarly, Excel will look for column headings (labels) without the need to select them.
3.	Click the `Insert` tab on the ribbon, then click the `PivotTable` button in the `Tables` group.
4.	In the `Create PivotTable` dialog box the PivotTable range is already selected.
5.	Click the radio button for `Existing Worksheet`, then click into the `Location box`.
6.	Click on cell `K2` to insert the PivotTable underneath its heading.
7.	The PivotTable placeholder is inserted, and the `PivotTable Fields` pane opens on the right.
8.	Click the checkbox next to the `Trimester label` and note that it is automatically added to the `Rows` box in the PivotTable Fields pane.
9.	Click and drag every Academic Group to the `Values` box.
  AEL
  Sciences
  Business
  Health
  Other L&T*
  RED**

Filtering
- In the PivotTable, click on the `arrowhead` in the `Row Labels` cell to explore the filtering options.{% endcapture %}
{% include card.md header="Activity : Data extraction with PivotTables" text=text %}

### Data ordering
You can add data in any order, or you can reorder it as you need.  Let’s do this to extract the data for attendance per skill group. 

{% capture text %}
1.	Click into cell `K8`.  Note that clicking away from the previous PivotTable closes the `PivotTable Fields` pane.  Clicking inside any PivotTable will open it again, or you can click the `Field List` button in the Show group on the `PivotTable Tools` contextual tab.
2.	In cell `K8` type `Attendance by Skill Group`.
3.	Select cells `A2:H10` as before.
4.	Click the `Insert` tab on the ribbon, then click the `PivotTable` button in the `Tables group`.
5.	Click the radio button for `Existing Worksheet`, click into the `Location` box then click on cell `K9` to insert the PivotTable underneath its heading.
6.	When the `PivotTable Fields` pane opens on the right, click and drag the `Skill Group` label to the Rows box.
7.	Now click and drag every `Academic Group` to the `Values` box, this time selecting them in ALPHABETICAL ORDER.
 AEL
 Business
 Health
 Other L&T*
 RED**
 Sciences{% endcapture %}
{% include card.md header="Activity : Data ordering in PivotTables" text=text %}

-----

### Data preview

OpenRefine gives you a preview to show you how it has interpreted the file you have uploaded or imported. If your data was tab-delimited rather than comma-delimited, the preview might look strange. 
- Be sure the correct separator is displayed in the box shown. 
- If you have made any changes, click `Update Preview` (bottom left). 
- If the wrong file is displaying, click `<<Start Over` (upper left).

There are options to indicate whether the dataset has column headers included and whether OpenRefine should skip a number of rows before reading the data. 
- Choose `UTF8` as the method of encoding as this should convert any 'smart' formatting into plain text.
- Make sure `Trim leading & trailing whitespace from strings` is checked. This will automatically remove any whitespace from the beginning or end of data strings or cells, making the data computer readible. Words with spaces at the beginning or end are particularly hard for we humans to tell from strings, but the blank characters will make a difference to the computer.
- Ensure the first row is used to create the column headings by checking the box `Parse next 1 line(s) as column headers`
- Make sure the `Parse cell text into numbers, dates,` ... box is not checked, so OpenRefine doesn't try to automatically detect numbers. Parsing in this context refers to the way the software will interpret the format of the data.
- Give the project a meaningful name such as `TrafficAccidentsCleanV1`
- If all looks fine, click `Create Project`.

{% include figure.html img="20201209_OR_Preview_Screen.png" alt="Create Project" caption="Create a project in OpenRefine" width="75%" %}

{% include button.md text="Watch the steps above on this video" link="https://vimeo.com/412189056/0d9031def0" color="info" %}



{% capture alert %}Note: Keep the terminal window hosting Java open in the background.{% endcapture %} {% include alert.md text=alert color="warning" %} 

-----

<p align="center">
  <a href="https://griffithunilibrary.github.io/intro-data-wrangle/content/1-intro.html"><-- BACK</a> |
  <a href="https://griffithunilibrary.github.io/intro-data-wrangle/content/3-lesson.html">NEXT --></a>
</p>

