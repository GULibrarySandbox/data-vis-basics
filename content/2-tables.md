---
title: Tables
nav: true
---

# Data visualisation using Microsoft Excel

## Part one: Tables

{% include figure.html img="2021_Excel-data-visualisation_Student-workbook.jpg " alt="Data visualisation using Excel" caption="Data visualisation using Excel" width="100%" %}

### Overview

Undertake the activities below to create PivotTables and PivotCharts.

{% capture text %}
- download activity .xls dataset from Griffith University's Research Data Storage [here](https://research-storage.griffith.edu.au/owncloud/index.php/s/7VHsCVyUsAKsTll)
- Open in MS Excel software{% endcapture %}
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
  - AEL
  - Sciences
  - Business
  - Health
  - Other L&T*
  - RED**

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
  - AEL
  - Business
  - Health
  - Other L&T*
  - RED**
  - Sciences
 
#### Reordering

Reordering 
If you hadn’t selected in the exact order you wanted or just changed your mind, you can still reorder the columns: 

#### Method A: click and drag

8.	In the `Values` box in the `PivotTable Fields` pane, point the mouse to the `Other L&T` label until the four-headed arrow `Move` shape appears.
9.	Click and drag the field to the last position in the list.

#### Method B: menu selection

10.	In the `Values` box in the `PivotTable Fields` pane, point the mouse to the `RED` label and click on the selection list arrowhead on the right.
11.	Choose `Move to end`.{% endcapture %}
{% include card.md header="Activity : Data ordering in PivotTables" text=text %}

-----

### Combining fields

In this data, both `Other L&T` and `RED` are categories, rather than Academic Groups. They don’t need to be shown as two separate fields. 

{% capture text %}
1.	Click in the `Sum of RED` heading (the last column in the PivotTable).
2.	On the `PivotTable Tools` tab on the ribbon, click on `Analyze` (should already be selected).
3.	Click on the `Fields, Items & Sets` button in the `Calculations` group.
4.	Click on `Calculated field`…
5.	Type a name for the field – e.g. `Other`.
6.	In the `Formula` field, leave the equals `(=)`, then select `Other L&T` and click `Insert` Field, type
`<space>+<space>`, then select `RED` and click `Insert Field`.
7.	Click `OK`.
8.	You can now remove `Other L&T` and `RED` from the Values box by `unchecking the boxes` for those fields.{% endcapture %}
{% include card.md header="Activity : Combining fields in PivotTables" text=text %}

### Renaming fields

You can rename fields in a PivotTable using any name except the original.  This looks more professional than each label being prefixed with “sum of” and also creates a more readable legend if you are also intending to create a chart. 

{% capture text %}
1.	In the `Values` box in the `PivotTable Fields` pane, point the mouse to the `Sum of AEL` label and click on the selection list arrowhead.
2.	Click on `Value Field Settings`…
   - NOTE:  You cannot use any name that is already used in the data table (i.e. “AEL”), but you can add a space to the end of the name which makes it different for Excel’s criteria, yet it looks the same to the reader.
3.	In the `Custom Name:` field, type `AEL<space>`.
4.	Click `OK`.
5.	Do the same for the other field values.{% endcapture %}
{% include card.md header="Activity : Renaming fields" text=text %}

Follow each activity in this video. 

<div class='embed-container'><iframe width="854" height="480" src='https://player.vimeo.com/video/428348749' frameborder='0' webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe></div>

-----

<p align="center">
  <a href="https://griffithunilibrary.github.io/data-vis-basics/content/1-rules.html"><-- BACK</a> |
  <a href="https://griffithunilibrary.github.io/data-vis-basics/content/3-charts.html">NEXT --></a>
</p>

