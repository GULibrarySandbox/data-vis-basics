---
title: Voyant
nav: true
---

# Voyant Tools

-----

[voyant-tools.org](voyant-tools.org) is a plug and play tool for simple text analysis and visualisation.   Voyant Tools will read and analyse a variety of documents types.  You can upload single or multiple PDFs, insert mulitple URLs or copy and paste text into the search box. 

Voyant Tools is an open-source project and the code is available through GitHub.  The code is under a GPL3 license and the content is under a Creative Commons By Attribution license.   It is a scholarly project that is designed to facilitate reading and interpretive practices for digital humanities students and scholars as well as for the general public.

Do not use personal, confidential or sensitive data in Voyant Tools.

## Features include:

- Cirrus: a word cloud showing the most frequent terms
- Reader: an efficient corpus reader that fetches segments of text as you scroll
- Trends: a distribution graph showing terms across the corpus (or terms within a document)
- Summary: a tool that provides a simple, textual overview of the current corpus
- Contexts: a concordance that shows each occurrence of a keyword with a bit of surrounding context
- and [more](https://voyant-tools.org/docs/#!/guide/tools)...

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


## Analyse the Visualisations

The standard visualisations will show basic Cirrus clouds and document terms count.  
The interactive reader in the centre of the screen shows the original source materials with individual terms in different colours.
To explore individual terms, click on a term in the reader and see counts and usage of the term in the Contexts box.  
The summary box displays the number of documents being examined, the total word count, unique words, vocab density, average words per sentence and a list of most frequent words in the corpus.
{% include figure.html img="voyant_screen.jpg" alt="voyant_analysis" caption="analysis" width="100%" %}


{% capture text %}
## Change the Visulations

Hover the mouse over the top of the section you wish to change  

click on the window button
scroll down the menus to choose the visualisation you need, there are two parts to this, a tools menu and visualisation type
click your desired option to select your visualisation

{% endcapture %}
{% include card.md header="Activity - Change the visualisations" text=text %}

## Export your findings
Step 5. Export
to export Voyant visualisations, hover the mouse along the top bar of the section you wish to export, you will see three icons in the image appear 
select the first icon, the square with the arrow, this will open a pop up window
the first option will give you the options to export HTML code, a bibliographic reference and a notebook;  the second option will give you a visualisation
select what you need and click export. 

## Cite your findings
to cite Voyant visualisations, hover the mouse along the top bar of the section you wish to export, you will see three icons appear 
select the first icon , it is a little square with an arrow , this will open a pop up menu
the first option here will give you the options for HTML code, a bibliographic reference and a notebook
click the bibliographic reference button then click export
there are three reference options available, copy the style you need. 

{% capture text %}

## Activities - Export and Cite your data
The key feature of Voyant is to be able to quickly create visual data, and then the capacity to choose your own visualisation and export the image for further use. 

In this set of activitis we will look at the different types of resources to upload and how to change the visualisations. 

Part 1 - Step 1 

Upload a variety of documents to Voyant

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
finally, again using the export function, export the bibliographic reference. 

{% endcapture %}
{% include card.md header="Export and Cite your data" text=text %}

## Voyant in practice- Articles citing Voyant Tools
To see how reserachers are using Voyant in their studies take a look at the following articles;

Stephanie Posthumus & Stéfan Sinclair(2014) Reading environment(s): digital humanities meets eco-criticism, Green Letters,18:3,254-273,DOI: 10.1080/14688417.2014.966737  (access via Griffith Library here)
Rambsy, K. (2016). Text-Mining Short Fiction by Zora Neale Hurston and Richard Wright using Voyant Tools. CLA Journal, 59(3), 251-258. Retrieved June 16, 2020, from www.jstor.org/stable/44325917 (access via Griffith Library here)





{% include button.md text="back to main" link="https://griffithunilibrary.github.io/data-vis-basics/" color="info" %}



<p align="center">
  <a href="https://griffithunilibrary.github.io/intro-data-wrangle/content/3-lesson.html"><-- BACK</a> |
  <a href="https://griffithunilibrary.github.io/intro-data-wrangle/content/5-lesson.html">NEXT --></a>
</p>
  
  
