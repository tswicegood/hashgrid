\#grid
======

A little tool that inserts a layout grid in web pages, allows you to fix it in place, and toggle between displaying it in the foreground or background.

Features

* Adaptable for all layout widths and alignments (this version assumes a 980px wide container including 20px gutters)
* Adaptable for any vertical rhythm value (this version assumes one lead of 20px)
* Show and hide, fix in place, or toggle foreground and background display using keyboard shortcuts
* Uses: A single JavaScript file, a few lines of CSS, and one image (for the vertical lines)

Notes on installation and usage can be found in the included index.htm file.

Installing Bookmarklet
----------------------
You can use #grid as a bookmarklet by adding a bookmark with the following JS:

    var stylesheet="http://github.com/tswicegood/hashgrid/raw/master/hashgrid.css";
    $('body').append($('<link rel="stylesheet" type="text/css" href="'+stylesheet+'"/>'));
    var url="http://github.com/tswicegood/hashgrid/raw/master/hashgrid.js";
    $.getScript(url,function(){var grid = new GridOverlay('grid');});

