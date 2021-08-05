---
title: Voyant
nav: true
---

# Voyant Tools

-----

[voyant-tools.org](voyant-tools.org) is a plug and play tool for simple text analysis and visualisation.   Voyant Tools will read and analyse a variety of documents types.  You can upload single or multiple PDFs, insert mulitple URLs or copy and paste text into the search box. After analysis work, image files of visualisatios can be exported for further use.

Voyant Tools is an open-source project and the code is available through GitHub.  The code is under a GPL3 license and the content is under a Creative Commons By Attribution license.   It is a scholarly project that is designed to facilitate reading and interpretive practices for digital humanities students and scholars as well as for the general public.

Do not use personal, confidential or sensitive data in Voyant Tools.

{% include figure.html img="VoyantTools.png" alt="Voyant tools list" caption="Voyant tools" width="100%" %}  
 

{% capture alert %}Cite the tool's developers when publishing a visualisation created using Voyant Tools:

`Sinclair, S. & Rockwell, G. (2016). Voyant Tools. Web. http://voyant-tools.org`
{% endcapture %}
{% include alert.md text=alert color="warning" %}



## How to use voyant tools

Paste the URLs or text you wish to analyse into the text box. You can also upload PDF, MS Word, .txt and other text files using the upload button. You can even analyse text from spreadsheets .xls, .csv, or JSON or XML files.

Watch the following videos on the different methods to upload content. Then choose a method in the activity below to upload some text.

This video shows how to upload mulitple URLS to Voyant. 
<iframe src="https://player.vimeo.com/video/563468503" width="640" height="564" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe>

This video shows how to copy and paste text into Voyant.
<iframe src="https://player.vimeo.com/video/563467758" width="640" height="564" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe>

{% capture text %}
To upload text:
- `copy` text from a document you wish to analyse
- `paste` the text into the `Add Texts` window
- click on `reveal`

To upload entire webpages:
- `copy` a URL or the multiple URLs you wish to analyse, add as many as required
- `paste` the URL/s into the `Add Texts` window
- click on `reveal`

To upload files from your computer:
- click on the `upload` button,  your files window will open
- Select file or files to anlayse 
- Click `open`
This will automatically open your selected files in Voyant.

Note what happens if you chose mulitple file types?{% endcapture %}{% include card.md header="Activity: uploading different text formats" text=text %}

Watch the Video, this will show you how to use Voyant tools, export your visualisation and cite your work
<iframe width="560" height="315" src="https://player.vimeo.com/video/563076024?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" title="voyant_URL_upload_tailed.mp4"></iframe>

-----
<p>
 
 </p>

## Analyse and export visualisations

{% include figure.html img="VoyantToolsAnalysisScreen.png" alt="Voyant analysis" caption="analysis screen of Voyant" width="100%" %}

Once uploaded the text is shown in an analysis and visualisation screen. 

The standard visualisations show the following in separate windows:
- Cirrus: a word cloud showing the most frequent terms in the corpus (top left window)
- Reader: a corpus reader that fetches segments of text as you scroll (center window)
- Trends: a distribution graph showing terms across the corpus (or terms within a document) (top right window)
- Summary: a tool that provides a simple, quantitative summary of the corpus (bottom left window)
- Contexts: a concordance that shows each occurrence of a keyword with a bit of surrounding context (bottom right window)

{% capture text %}
- To explore individual terms, click on a term in the reader and see counts and usage of the term in the Contexts box.  
- The summary box displays the number of documents being examined, the total word count, unique words, vocab density, average words per sentence and a list of most frequent words in the corpus.{% endcapture %}{% include card.md header="Activity - Explore the text" text=text %}

{% capture text %}
{% include figure.html img="VoyantChangeTools.png" alt="How to change the analysis tool in Voyant" caption="How to change the analysis tool in Voyant" width="100%" %}
- Hover the mouse over the top of the analysis window section you wish to change  
- click on the `window` button
- Scroll down the menu to choose the visualisation you need, there are two parts to this, a tools menu and visualisation type
- Click your desired option to select your visualisation{% endcapture %}{% include card.md header="Activity - Change the visualisation" text=text %}

{% capture text %}
{% include figure.html img="VoyantExportButton.png" alt="Export button" caption="Voyant's export button" width="100%" %}
- Hover the mouse along the top bar of the section you wish to export, you will see three icons in the image appear 
- Select the first icon, the square with the arrow, this will open a pop up window
{% include figure.html img="VoyantExportPopUp.png" alt="Export button" caption="Voyant's export options" width="100%" %}
- the first option will give you the options to export HTML code, a bibliographic reference and a notebook
- to copy a reference click the bibliographic reference button then click export
- there are three reference options available, copy the style you need. 
{% include figure.html img="VoyantExportReference.png" alt="Export Voyant reference" caption="Export a reference to Voyant" width="100%" %}
- Select the second option for an image file
{% include figure.html img="VoyantExportVis.png" alt="Select Export Visualisation" caption="Select Export Visualisation" width="100%" %}
- Choose the `file type`, then click `export`, and `right click` on the `Thumbnail image`
- Select `Save image as...`
- name the image file
- `Save`
{% include figure.html img="VoyantExportPNG.png" alt="Export an image from Voyant" caption="Export an image Voyant" width="100%" %}{% endcapture %}{% include card.md header="Activity - Export your findings" text=text %}

{% capture text %}
In this set of activities we will look at the different types of resources to upload and how to change the visualisations. 

Part 1 - Step 1 

- Upload a variety of documents to Voyant

In the lesson we uploaded URLs, PDFS and text to the tool, now try adding both text and a URL to the 'Add Texts' box
does the tool read both elements? 
Step 2

Upload saved PDFs -  using the upload tab, upload multiple PDF documents 
notice how the reader separates the individual articles in the reader by colour
in document, click on a term, notice how the trends map and contexts box change
find your key themes in the text and to track how these terms are used in the text and the contexts. 

Part  2

with your data set, change the visualisation; using the corpus tools menu change the visualisation to 'Steam graph'
now export this using the export visualisation function, export the graph as an SNG, copy the visualisation and paste the image into a word doc
finally, again using the export function, export the bibliographic reference.{% endcapture %}{% include card.md header="Activity: Need to change this...." text=text %}

## Voyant in practice- Articles citing Voyant Tools

To see how reserachers are using Voyant in their studies take a look at the following articles:

- Posthumus, S. & Sinclair, S.(2014). Reading environment(s): digital humanities meets eco-criticism, *Green Letters*,18(3),254-273. [https://doi.org/10.1080/14688417.2014.966737](https://doi.org/10.1080/14688417.2014.966737)
- Rambsy, K. (2016). Text-Mining Short Fiction by Zora Neale Hurston and Richard Wright using Voyant Tools. *CLA Journal*, 59(3), 251-258. [www.jstor.org/stable/44325917](www.jstor.org/stable/44325917)

-----

<p align="center">
  <a href="https://griffithunilibrary.github.io/data-vis-basics/content/4-convert.html"><-- BACK</a> |
  <a href="https://griffithunilibrary.github.io/data-vis-basics/content/6-rawgraphs.html">NEXT --></a>
</p>
