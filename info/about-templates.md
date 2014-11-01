## A bit about templates.

#### Some reasons I think modular templates work better.
1. I find large monolithic chunks to have some severe downsides.
  * They are more difficult to update than modular templates.
  * They are more difficult to utilize for educational purposes.

2. Here are some upsides to using modular templates.
  * Easy to update specific parts of specific websites( update only the sidebar ).
    * Different Cascading Style Sheet calls per page allows for more efficient declarations and even possibly dynamic declarations requiring no modification created by directory depth.
  * Easy to use for educational purposes.
  * Easy to add modular content (add a new html/css module).
    * An example is the sidebar used in [my site](http://edge226.github.io).
      * sidebar.html gets written to the html file when a line including `<p>Sidebar.</p>` is found in index-template.html
  * Easy to pick and choose which parts of the site are the same and which are different among subsites.

#### Here is a table about the structure of the templates.

* The Write tag is used when writing html files.
* Read regex is used by the update-templates program when scanning and splitting apart the index.html file.
  * In the case of the Write tag or Read regex being Default it means the default behavior will be to write to that file.
  * In the case of it being blank I have not determined what is appropriate yet.

File | Write tag | Read regex | Purpose
----|----|----|----
index-template.html | Default | Default | This holds the core html that all other files are injected into to create the resulting html file.
meta.html | `<p>Meta.</p>` |  | Holds the meta information of the site.
css.html | `<p>Load CSS.</p>` | | Holds the CCS definitions of the site.
title.html | `<p>Title.</p>` | | Holds the title of the site
header.html | `<p>Header.</p>` | | Holds the header information of the site.
downloads.html | `<p>Downloads.</p>` | | Holds the download buttoms used at the top of the site.
sidebar.html | `<p>Sidebar.</p>` | | Holds the html for a side bar if any.
*.md | `<p>Template.</p>` | | Contains the main content of the resulting generated html file.
javascript.html | `<p>Javascript.</p>` | | Contains java script definitions.
