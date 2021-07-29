---
title: Export
nav: true
---

# Export and convert chart to publication quality image

------

### Image formats

Some publishers require that you submit images from a select range of formats only. For example, instructions from Wiley include:
- Use the following standard image formats: `BMP`, `JPG`, `JPEG`, `TIF`, `WMF`, or `EPS`.

In this group, the first four are `Raster` formats, while the last two are `Vector` formats. When saving an image you should choose a `Raster` format wherever possible as Raster images are more flexible and resizable without loss. Make sure to refer to the journal’s style guide for preferred formats.

-----

### Image resolution

In addition, manuscripts or journals require images with high resolution, nominally `300 ppi` (pixels per inch).

Using Cut and Paste from Excel to Word results in a poor-quality image (72-96 ppi), often with bad pixellation particularly when resizing the image.

There are some things you can do to improve the quality of images in your document.

-----

### Creating suitable images

The best way to create a quality graphic is to use a graphic editor. Below is a list of popular editors.

- `Photoshop` : (*staff only*) a component of the `Adobe Creative Cloud` suite of programs. Find it under `Installable Applications` on your Griffith computer. 
- `GNU Image Manipulation Program (GIMP)`[https://www.gimp.org/](https://www.gimp.org/) : open source (free) (GNU/Linux, OS X, Windows and other operating systems).
- `PhotoPad`[https://www.nchsoftware.com/photoeditor/](https://www.nchsoftware.com/photoeditor/)` : free for non commercial users (Windows)
- `Preview` (Mac OS) 

{% capture text %}
1. Click the `Start` button on your computer.
2. If you see the `Adobe Creative Cloud` shortcut, click on it to install `Photoshop CC`. (You may like to explore some of the other available applications later.)
OR
3. If you don’t see Adobe Creative Cloud in your Start menu, go to Griffith’s `Adobe Product Access` web page:
  - [https://intranet.secure.griffith.edu.au/computing/software/self-help-and-support/general-information/adobe-licensing-changes](
https://intranet.secure.griffith.edu.au/computing/software/self-help-and-support/general-information/adobe-licensing-changes)
4. Follow the instructions to download and install the software.{% endcapture %} {% include card.md header="Activity - Accessing Photoshop (staff)" text=text %}

##### 

{% capture text %}
1. Generate your chart in Excel.
2. Right-click on the chart, then click on `Save As Picture`.
3. In the `Save as type`: selection list, choose `JPEG` (`*.JPG,*.JPEG,*.JPE`) (or file type nominated in the journal’s style guide).
4. Browse to the location to save to, then click `Save`.
5. Click `OK` in the `JPEG Options` dialog box.

NOTE: If you have the option to submit `*.PNG` files, this is a better format than JPEG as the file size is smaller.

6. Close Excel and refer to the handout 2021_Excel-data-visualisation_Increase-Resolution.docx for instructions on how to enhance the image using alternative software.{% endcapture %} {% include card.md header="Activity  - Save the chart as an image" text=text %}


Faceting and filtering look very similar. A good distinction is that faceting gives you an overview, description and count of all of the data that is currently selected, while filtering allows you to select a subset of your data by a string - of text in this case - for analysis or cleaning.

{% include button.md text="Watch this video on filtering" link="https://vimeo.com/412533690/80c2ae057e" color="info" %}

------

### Sorting data

Using `Crash_Street`, let's explore data using sorting.

{% capture text %}
- In  `Crash_Street`  column select drop-down menu and  `Sort`.   Options include:
  - Sort by text
  - Sort by numbers
  - Sort by dates
  - Sort by booleans (TRUE or FALSE values). 
- Select  `text`
- Additional options will then appear for you to fine-tune your sorting, select  `a-z`
- You can also specify what order to put *blanks* and *errors* in the sorted results.
-  `Ok`

When performing the first sort, you will notice the drop-down menu for the selected column shows  `Sort ...` 

If you try to re-sort a column that you have already used, the drop-down menu changes slightly, to  `> Sort`  without the  `...`, to remind you that you have already used this column. Additional options include:

  - `Sort > Sort ...` - This option enables you to modify your original sort.
  - `Sort > Reverse` - This option allows you to reverse the order of the sort.
  - `Sort > Remove sort` - This option allows you to undo your sort.
- Remove this sort.{% endcapture %} {% include card.md header="Activity - sort by text" text=text %}

### Sort by multiple columns

You can also sort by multiple columns and this makes it easier to explore data easily before analysis and processing. Do this by performing a sort on additional columns.

The sort results will depend on the order in which you select columns to sort.

To restart the sorting process with a specific column, check the  `sort by this column alone`  box in the  *Sort pop-up menu*.

If you go back to one of the already sorted columns and select `Sort > Remove sort` , that column is removed from your multiple sort. If it is the only column sorted, then data reverts to its original order.

{% capture text %}
- Sort  `Crash_Street` again, select  `Sort... > text and a-z`
- Add an additional sort by  `Crash_Street_Intersection`, select  `Sort... > text and a-z`
- Examine the first page of results for multiple accidents at the same location
- Remove sort{% endcapture %} {% include card.md header="Activity - sort by multiple columns" text=text %}

Sorts in OpenRefine are temporary. If you remove the Sort, the data will go back to its original unordered state.

The Sort drop-down menu at the top of the screen also lets you amend the existing sort to:
- Reverse the sort order
- Remove existing sorts
- Reorder rows permanently.

### Find and fix missing values by sorting

Let's try to find if there are missing values for the `Crash_Longitude` variable.

{% capture text %}
- In  `Crash_Longitude column`, select  `Sort... > numbers` 
- in pop up box select  `smallest first` and reposition  `Errors` &  `Blanks` to the top of the column.
- `Ok`
- Notice the first value is missing, from record *243929*.

You may want to map this data later, so it is important to have complete latitude and longitude information.  You may be able to identify the missing value by other variable attributes.  

When you know your data or look at the variable in context with other similar observations you can identify what type of data problem might be occurring and possible solutions.  

In this case, you could search other variables such as  `Crash_Street` ,  `Crash_Street_Intersection`  and  `Suburb_PostCode` to identify similar locations.

Find the missing `Crash_Longitude` value for record *243929*. There are a few possibilities.  This is one....

- Write down the values in the  `columns Crash_Street` ,  `Crash_Street_Intersection`  and  `Suburb_PostCode` , for record *243929*
  - Values are: *Mary St; Miles St; Mount Isa City, (4825)*
- Remove the sort.
- Filter  `Crash_Street`  by *Mary*
- Filter  `Crash_Street_Intersection`  by *Miles St*
- Examine results for similarities
- Copy and paste the missing `Crash_Longitude`  value to record *243929*.{% endcapture %} {% include card.md header="Activity - find & fix missing values by sorting" text=text %}


{% include button.md text="See the steps in this video" link="https://vimeo.com/412602729/e3da0ba711" color="info" %}

<p>
</p>

{% capture text %}
There is another method you could use to find a missing value, that we have used, what is it?
{% include modal.md button="Quiz 2 Solution" color="success" title="Quiz 2 Solutions" text="Select  `Facet > Customized facets > Facet by Blank or Null`." %}{% endcapture %} {% include card.md header="Quiz 2. Another method to find missing data in Crash_Longitude column?" text=text %}

-----

<p align="center">
  <a href="https://griffithunilibrary.github.io/intro-data-wrangle/content/4-lesson.html"><-- BACK</a> |
  <a href="https://griffithunilibrary.github.io/intro-data-wrangle/content/6-lesson.html">NEXT --></a>
</p>

