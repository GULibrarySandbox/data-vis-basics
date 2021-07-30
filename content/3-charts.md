---
title: Charts
nav: true
---

# Data visualisation using Microsoft Excel 

## Part two: Charts

-----

You don’t need a PivotTable to create a chart – charts can be created from any raw data – but, as per the previous exercises, your writing will generally deal with one aspect of the data at a time, so the figures created for inclusion in each section should represent that single discussion. 

{% capture text %}
1.	Select cells `K10:P12`.
2.	Click the `Insert` tab on the ribbon.
3.	Click `Column or Bar Chart`.  Choose `2-D column`.
4.	The chart is referred to as a `PivotChart` because it is based on a PivotTable.{% endcapture %} 
{% include card.md header="Activity : Creating a chart" text=text %}

{% include figure.html img="2021_Excel-data-visualisation_Student-workbook.jpg " alt="PivotChart" caption="PivotChart" width="100%" %}

Follow the activity to create a PivotChart in this video.

<iframe src="https://player.vimeo.com/video/428348675" width="640" height="564" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe>

-----

## Rules for publication-quality visualisations

Excel produces an aesthetically pleasing chart that is formatted according to the theme of your workbook, but there are specific rules used to create publication-quality visuals which means some editing of your chart.

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

-----

## Chart tools

The following sections describe how to prepare your chart for publication. 


#### Tool: PivotChart Tools tab

When the chart is selected, the `PivotChart Tools` contextual tab is added to the ribbon. There are three groups of commands on this contextual tab: `Analyze` – `Design` – `Format`.


##### Rule 1 – Start with a clean chart
{% capture text %}
Hide the PivotChart fields

1. Click on the `Analyze` group on the `PivotChart Tools` contextual tab if not already selected.
2. Click on `Field Buttons`, then click on `Hide All`.{% endcapture %} 
{% include card.md header="Activity : PivotChart Tools tab – Field buttons" text=text %}


##### Rule 2 – Remove the gap between the columns in a column chart
{% capture text %}
Chart Style

1. Click on the `Design` tab on the `PivotChart Tools` contextual tab.
2. Mouse over the `Chart Styles gallery` to view available styles, clicking on the `More` button to expand the gallery.
3. Select `Style 11`. {% endcapture %} 
{% include card.md header="Activity : PivotChart Tools tab – Chart style" text=text %}

-----

#### Tool: Double-click or right-click

All the chart components can be edited by either double-clicking on the element within the chart or by right-clicking on it.

##### Rule 3 - No colour – use white/grey/black

While some publications are printed in full colour this can be a very expensive practice and the alternative of printing colour in black and white may not give satisfactory results when converted to shades of grey by an unknown conversion process. It is better to control this process yourself.

{% capture text %}
1. Click on the `PivotChart`, then double-click on the legend entry for `AEL` to open the `Format Legend Entry` pane.
2. Click on `Fill`.
3. Choose `Solid Fill`.
4. Choose `White` as the `Fill colour`. (Note: When the fill colour is white, there should be a black border).
5. Click on `Border`.
6. Choose `Solid Line`.
7. Choose `Black` as the colour.
8. Close the pane.
9. Now double-click on the legend entry for `Business` to open the `Format Legend Entry` pane.
10. Click on `Fill`.
11. Choose `Solid Fill`.
12. Choose a medium-grey colour (e.g. `White, Background 1, Darker 25%`) as the `Fill colour`. (Note: When the fill colour is anything other than white, there should be no border).
13. Click on `Border`.
14. Choose `No Line`.
15. Close the pane.
16. Change the fill colour for `Health` and `Sciences`, incrementing the colours in shades of grey (no border is required for grey shades).
17. Change the fill colour for `Other` to `black` (no border).{% endcapture %} 
{% include card.md header="Activity : Double-click or right-click elements - Colours" text=text %}

-----

#### Tool: Chart Elements

Many formatting commands are featured in the `Chart Elements` menu which is shown as a green “plus” sign beside the chart itself.

##### Rule 4 - Legend to be displayed at the top-right of the chart
{% capture text %}
Legend
1. Click on the PivotChart.
2. Click on `Chart Elements` (the green plus sign).
3. Point the mouse to `Legend`, then click on the `More` arrowhead.
4. Click on `More options…` to open the `Format Legend` pane.
5. Click the radio button for `Top Right`.
6. Close the pane.{% endcapture %} 
{% include card.md header="Activity : Chart Elements tool - Legend" text=text %}

##### Rule 5 - Enhance the horizontal axis bar settings
{% capture text %}
Major Gridlines (horizontal)
1. Click on the PivotChart.
2. Click on `Chart Elements` (the green plus sign).
3. Point the mouse to `Gridlines`, then click on the `More` arrowhead.
4. Click on `More options…`.
5. Click the selection list arrow beside `Major Gridline Options`.
6. Click on `Horizontal (Category) axis`.
7. Under `Line`, choose `Solid line`, then choose `Colour` = `black` and `size` (e.g. `2pt`).
8. Close the pane.{% endcapture %} 
{% include card.md header="Activity : Chart Elements tool – Horizontal axis" text=text %}

##### Rule 6 - Enhance the vertical axis bar to match the horizontal
{% capture text %}
Major Gridlines (vertical)
1. Click on the PivotChart.
2. Click on `Chart Elements` (the green plus sign).
3. Point the mouse to `Gridlines`, then click on the `More` arrowhead.
4. Click on `More options…`.
5. Click the selection list arrow beside `Major Gridline Options`.
6. Click on `Vertical (Category) axis`.
7. Under `Line`, choose `Solid line`, then choose `Colour` = `black` and `size` (e.g. `2pt`).
8. Click on the `Axis Options` button (the green button that looks like a bar chart)
9. Click on `Tick Marks` to open the settings.
10. For `Major type`, choose `Outside`.
11. Close the pane.{% endcapture %} 
{% include card.md header="Activity : Chart Elements tool – Vertical axis" text=text %}

##### Rule 7 - No background grid
{% capture text %}
Background Gridlines
1. Click on the PivotChart.
2. Click on `Chart Elements` (the green plus sign).
3. Uncheck the box for `Gridlines`.{% endcapture %} 
{% include card.md header="Activity : Chart Elements tool – Gridlines" text=text %}

##### Rule 8 - Add error bars

Error bars are mostly used for scientific data and may not apply to all.
If error bars are used, they must be described in the Figure caption in the document.
{% capture text %}
1. Click on the PivotChart.
2. Click on `Chart Elements` (the green plus sign).
3. Point the mouse to `Error Bars`, then click on the `More` arrowhead.
4. Click on `Standard Deviation`.
5. Close the pane.{% endcapture %} 
{% include card.md header="Activity : Chart Elements tool – Error bars" text=text %}


##### Rule 9 - Add axis titles
{% capture text %}
1. Click on the PivotChart.
2. Click on `Chart Elements` (the green plus sign).
3. Check the box for `Axis Titles`.
4. Double-click into the vertical axis title and type `Attendance`.
5. Double-click into the horizontal axis title and type `Skill Group`.{% endcapture %} 
{% include card.md header="Activity : Chart Elements tool – Axis titles" text=text %}

##### Rule 10 - Use a large clear font

Use a font that complements your document, e.g. Times New Roman to match the body of the document or Arial to match headings in your document.
{% capture text %}
1. Select the text in the `vertical axis title`, then click on the `Home` tab on the ribbon.
2. Click the `Font Settings` option button.
3. Uncheck the `All Caps` option.
4. Choose a suitable `font` and `font size` for the text (e.g. to match your document – `Times New Roman, 14`).
5. Do the same for the `horizontal axis title`.
6. Adjust other text areas such as the `vertical axis values`, the `horizontal axis values` and the `legend`.{% endcapture %} 
{% include card.md header="Activity : PivotChart text elements" text=text %}

##### Rule 11 - Adjusting PivotChart values
{% capture text %}
1. In the PivotChart, click on the `Vertical (value) axis`, then right-click on it.
2. Click on `Format Axis…`
3. In the `Format Axis` pane, under `Bounds`, set the minimum to `0` (zero) and the maximum values to just above the highest value in the data range (for this exercise, `240`).
4. Close the pane.{% endcapture %} 
{% include card.md header="Activity : Adjusting PivotChart values" text=text %}

##### Rule 12 - No border

Charts should have no border in the publication, so remove this as a last step.
{% capture text %}
1. Double-click on the PivotChart.
2. In the Format Chart Area pane, under Border, check the radio button for No line.
3. Close the pane.{% endcapture %} 
{% include card.md header="Activity : Remove the PivotChart border" text=text %}

#### Resize the chart

Excel’s graphical user interface (GUI) allows for resizing of the chart without distorting the content. The chart will not retain this quality once exported from Excel, so resize the image to a suitable size that:
  (a) won’t need too much resizing in the Word document; and
  (b) can be applied to every chart created to maintain consistency
  
{% capture text %}
1. Decide on a good size for your chart (e.g. 9cm (h) x 15cm (w)).
2. Use the resize handles to manually resize the chart. To maintain perspective, hold down the <Shift> key as you drag.
OR
3. Click on the Format group on the PivotChart Tools contextual tab and adjust the sizing numerically in the Size group.
4. Take note of the physical dimensions so you can apply the same dimensions to other charts.{% endcapture %} 
{% include card.md header="Activity : Resize the chart" text=text %}
  
*Format video here*
  
##### Save chart as an image
  
{% capture text %}
1. Generate your chart in Excel.
2. Right-click on the chart, then click on `Save As Picture`.
3. In the `Save as type`: selection list, choose `JPEG` (`*.JPG,*.JPEG,*.JPE`) (or file type nominated in the journal’s style guide).
4. Browse to the location to save to, then click `Save`.
5. Click `OK` in the `JPEG Options` dialog box.
6. Close Excel.{% endcapture %} {% include card.md header="Activity - Save the chart as an image" text=text %}

-----

<p align="center">
  <a href="https://griffithunilibrary.github.io/intro-data-wrangle/content/2-tables.html"><-- BACK</a> |
  <a href="https://griffithunilibrary.github.io/intro-data-wrangle/content/4-lesson.html">NEXT --></a>
</p>
