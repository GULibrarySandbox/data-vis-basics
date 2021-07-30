---
title: Convert
nav: true
---

# Create a publication quality image

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

### Image editing software

The best way to create a quality graphic is to use a graphic editor. Below is a list of popular editors.

Download and install one of these tools to suit your computer's operating system, then follow an activity below to convert your chart or figure to an image of the correct resolution and file type.

- *Photoshop* : (*staff only*) part of Adobe Creative Cloud suite of programs 
- *GNU Image Manipulation Program (GIMP)* [https://www.gimp.org/](https://www.gimp.org/) : open source (free) (GNU/Linux, OS X, Windows and other operating systems)
- *PhotoPad* [https://www.nchsoftware.com/photoeditor/](https://www.nchsoftware.com/photoeditor/) : free for non commercial users (Windows)
- *Preview* (Mac OS) 

{% capture text %}
1. Click the `Start` button on your computer.
2. If you see the `Adobe Creative Cloud` shortcut, click on it to install `Photoshop CC`.
OR
3. If you don’t see Adobe Creative Cloud in your Start menu, go to Griffith’s `Adobe Product Access` [web page](https://intranet.secure.griffith.edu.au/computing/software/self-help-and-support/general-information/adobe-licensing-changes)
4. Follow the instructions to download and install the software.{% endcapture %} {% include card.md header="Activity - Accessing Photoshop (staff)" text=text %}

{% capture text %}
-	Generate your chart in Excel.
-	Select the chart and copy it to the clipboard (Copy or `<Ctrl>+<C>`).
-	Open *PhotoShop CC*.
-	In the Welcome screen, click on `Create New…`, or select `File` > `New`.  A `New Document` dialog box will open.
- In the `Preset Details` on the right-hand side, change the resolution to `300 pixels/inch` and click `Create`.  A canvas has been created that is the correct size for your chart.
{% include figure.html img="PhotoShop1.png" alt="PhotoShop software" caption="Create image using PhotoShop" width="70%" %}
-	Click `Edit` > `Paste` (or press `<Ctrl>+<V>`) to paste your chart onto the canvas, or drag and drop the file onto the canvas.
- Click `File` > `Export…` > `Quick Export as PNG` to save your edited image in the format specified by the journal’s style guide and in the appropriate location.
{% include figure.html img="PhotoShop2.png" alt="PhotoShop software" caption="Export image using PhotoShop" width="70%" %}{% endcapture %} {% include card.md header="Activity - Create image using PhotoShop CC" text=text %}
 
{% capture text %}
1.	Open *GIMP* and click on `File` > `Open` and browse to locate the image to be resized.
2.	With the image open, click on `Image` > `Scale Image` to open the `Scale Image` dialog box.
3. The `Image Dimensions` dialog box is opened.  Change both the `X` and `Y` resolutions to that specified by the journal’s style guide – usually `300 pixels/inch`.  You can also use `Image, Scale Image` again to change the dimensions of the image once the resolution has been set.
4. Click on the `File` > `Export` to save your edited image in the `format` specified by the journal’s style guide and in the appropriate location.
{% include figure.html img="GIMP2.png" alt="GIMP software" caption="Create image using GIMP" width="70%" %}{% endcapture %} {% include card.md header="Activity - Create image using GIMP" text=text %}

{% capture text %}
- Open *PhotoPad* Image Editor.
- Click on `Open` on the `Home` tab, then browse to locate the image to be resized.
- With the image open, click on `Resolution` on the `Home` tab.
{% include figure.html img="PhotoPad1.png" alt="PhotoPad software" caption="Create image using PhotoPad" width="100%" %}
- Change the resolution to that specified by the journal’s style guide – usually `300 pixels/inch`.
- Click the `Apply` button.  You can also change the dimensions of the image once the resolution has been set.
{% include figure.html img="PhotoPad2.png" alt="PhotoPad software" caption="Change resolution in PhotoPad" width="50%" %}
- Select `save` on the `Home` tab, then `Save As…` to save your edited image in the `format` specified by the journal’s style guide and in the appropriate location.
{% endcapture %} {% include card.md header="Activity - Create image using PhotoPad" text=text %}

{% capture text %}
1.	Go to the application folder on Mac and open `Preview`. Then click `File` on the menu bar and `Open…`.  
2.	Browse to locate the image to be resized.
3.	Open the image, click on `Tools` in the menu bar, select`Adjust Size`.
4. The `Image Dimensions` dialog box is opened.
5.	Change the resolution to that specified by the journal’s style guide – usually `300 pixels/inch`.
6.	Click `OK`.{% endcapture %} {% include card.md header="Activity - Create image using Preview (Mac OS)" text=text %}

{% capture alert %}*Note:* If you have the option to submit `*.PNG` files, this is a better format than JPEG as the file size is smaller.
{% endcapture %}
{% include alert.md text=alert color="warning" %}


-----

<p align="center">
  <a href="https://griffithunilibrary.github.io/intro-data-wrangle/content/4-lesson.html"><-- BACK</a> |
  <a href="https://griffithunilibrary.github.io/intro-data-wrangle/content/6-lesson.html">NEXT --></a>
</p>

