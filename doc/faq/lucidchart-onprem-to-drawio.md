---
title: Migrate from Lucidchart OnPrem to draw.io
layout: page
faq: true
categories: [Import, Lucidchart, Confluence Data Center and Server]
---

If you want to import a single Lucidchart diagram into draw.io, you can do this via copy and paste. But that's not efficient if your instance contains many Lucidchart diagrams.

draw.io has a mass import function that converts all of your Lucidchart OnPrem diagrams into the .drawio file format.

__Note:__ the Lucidchart to draw.io import is not 100% fidelity. These are different software products with different data models, so it never can be 100%. We have invested a lot of time to getting the import as close as possible.

You are welcome to report issues, still. Please understand that we’re at boundary cases now and generally we will be unable to improve the import much further. Keep this in mind when deciding whether or not to migrate to draw.io.

## Convert all of your Lucidchart OnPrem diagrams to .drawio diagrams

1. As an administrator, go to your Confluence Server instance's administration section, scroll down and click on the draw.io Add-On Configuration, in the left-hand panel.
2. Select the Lucidchart OnPrem Import tab.
<br /><img src="/assets/img/blog/lucidchart-onprem-import-start.png" style="max-width:100%;height:auto;" alt="Start the mass import of all Lucidchart OnPrem diagrams to draw.io in Confluence Server">
3. Click on the blue Start Import button. If you have a lot of Lucidchart diagrams in your instance, this can take some time. Ideally, run the import when few users are using the instance. You will see status updates as each diagram is imported.
<br /><img src="/assets/img/blog/lucidchart-onprem-import-report.png" style="max-width:100%;height:auto;" alt="Check the import report after the Lucidchart OnPrem mass import to draw.io in Confluence Server finished">

If you have previously run the Lucidchart mass import, the diagrams will not be imported a second time. In this case, you'll see a red error message. You can check the Confluence page that the diagram is on by searching for its title to make sure that the diagram was already converted to a draw.io diagram.

<img src="/assets/img/blog/lucidchart-onprem-import-skip-file.png" style="max-width:100%;height:auto;" alt="Previously converted diagrams from Lucidchart OnPrem to draw.io won't be converted again">

This mass import will import each diagram to the draw.io format, create a new page version and replace the embedded Lucidchart diagram on its page with the newly created draw.io diagram. The original Lucidchart diagram files are not deleted or changed in any way by this mass import. They will remain attached to their page.
