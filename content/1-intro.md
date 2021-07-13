---
title: Intro
nav: true
---
# Ten simple rules for better figures

-----

{% include figure.html img="OpenRefine.JPG" alt="OpenRefine software" caption="OpenRefine" width="100%" %}

[OpenRefine](http://openrefine.org) is a [Java](https://www.java.com/en/)-based program that runs on your computer (not online).

Adapted from: Rougier, N.P., Droettboom, M., Bourne, P.E. (2014). Ten Simple Rules for Better Figures.
PLOS Computational Biology 10(9): e1003833.[https://doi.org/10.1371/journal.pcbi.1003833](https://doi.org/10.1371/journal.pcbi.1003833)

{% capture text %}
1. **Know your audience**: a figure should be tailored to your audience and will likely be presented differently to groups including peers, students or the general public.
2. **Identify your message** before developing the figure. A figure is a quick way to introduce facts, or a result too complex to explain only with words.
3. **Adapt the figure to the support medium**. The reader of a journal article has time & the ability to zoom on a figure vs a conference attendee has limited time & the presentation is at a distance.
{% endcapture %} {% include card.md header="10 simple rules for better figures" text=text %}

{% capture text %}
- Split columns or rows of data up into more granular parts
- Combine multiple datasets into one
- Combine values from two or more variables (concatenation)
- Add new variables (columns) or observations (rows) to a dataset
- Reshape data from rows and columns to visualise data in a different arrangement
- Organise data{% endcapture %} {% include card.md header="Extend & transform data" text=text %}

{% capture text %}
- Sort by variables and values
- Agregrate: reorganise to get a summary of the data
- Filter: extract a subset by value
- Facet: summarise values to provide a big picture of your data or to identify outliers{% endcapture %} {% include card.md header="Explore data prior to analysis" text=text %}

{% capture text %}
- Document all steps taken to process the data
- Create scripts to automate and repeat the processes on other datasets{% endcapture %} {% include card.md header="Document & repeat steps" text=text %}

Explore the two figures below to see examples of messy and clean tabular data.

**Messy data example**
{% include figure.html img="MessyData.JPG" alt="Messy Data" caption="Messy Data" width="100%" %}

**Clean data example**
{% include figure.html img="TidyData.JPG" alt="Clean Data" caption="Clean Data" width="100%" %}


<p align="center">
  <a href="https://griffithunilibrary.github.io/intro-data-wrangle/content/0-setup.html"><-- BACK</a> |
  <a href="https://griffithunilibrary.github.io/intro-data-wrangle/content/2-lesson.html">NEXT --></a>
</p>

