 ####################
 #                  #
 #  CONTEXT V3.0.2  #
 #                  #
 ####################      Copyright Liam Goodacre, 2015-2018


This is a beta version of Context v3.0.2. There are still some bugs left and your help in tracking down both of these will be much appreciated.


SETUP:

Context runs on PD Vanilla V 0.47 or later. Once you have downloaded Context, you must declare its location so that PD knows how to find it on your computer. To do this, go to Edit --> Preferences --> Path --> New and select the location of Context's home folder.

EXTERNALS:

Externals are PD objects that are not available in PD Vanilla and must be installed seperately (Help --> Find Externals). Context relies heavily on externals (see LIST OF EXTERNAL LIBRARIES below). To make setup at easy as possible, Context distributes with all its external dependencies, according to the terms of their various licenses. This means that Context should work "out of the box" without the user having to manually download and declare external libraries.

There are some reasons why you might not want to use the externals which are distributed with Context. For instance, you might find that your patches are reverting to an unwanted version of an external object, if you have a different version of a library that the one Context is using. If you want to avoid the externals that are distributed with Context, or if you find that they are not working, simply delete or rename the following folders from the main Context folder: "cyclone", "else", "flatgui", "hcs", "iemguts", "iemmatrix" "list-abs", and "zexy". (Do not delete "ctxfiles" or "helpfiles"!) Context will now look for its external objects in your usual search directories, so make sure that your libraries are in order inside your "PD Documents Directory" or in another search path.


You should also consider adding the text "-font-face normal" into the startup flags (Edit --> preferences --> Startup --> Startput Path). This fixes a bug in 0.47 where the text is bolded, which throws the float and symbol atom off in the main GUI. Hopefully this won't be necessary in later releases.


MIASCELLANEOUS:

Context does not currently work on L2Ork or Purr Data.

Context patches sometimes take a long time to load (some of them several minutes). You can speed this up by turning off DSP before loading, then turning it back on. Faster machines are recommended.

Different installations sometimes have different font sizes, which throws off the alignment of the float- and symbol-atoms on the Context GUI. You can (hopefully) fix this annoyance in the [config] file in the main folder. If the atoms are not perfectly conjoined, then open the config.pd file and change the connection from "bold" to "thin" or vice versa. I can't guarantee that this will accomodate every system though. If you're still having trouble, please report a bug.

You should also consider adding the text "-font-face normal" into the startup flags (Edit --> preferences --> Startup --> Startput Path). This fixes a bug in 0.47 where the text is bolded, which throws the float and symbol atom off in the main GUI. Hopefully this won't be necessary in later releases.


DOCUMENTATION:

There are four parts to the Documentation:

1. The Context Manual. This is included in this folder as an odt and pdf. This is the most comprehensive guide of what Context is and how to use it.
2. Examples files, housed in the 'helpfiles' folder. These reference the manual and are meant to be studied in parallel with it.
3. Help prompts built into the Context menu. You can access these from within PD by right clicking on Context, selecting "properties" and clicking on the last item on every page (except the first one).
4. video tutorials at https://www.youtube.com/channel/UC_9u0n_ugUW7OjWrJRvhTjA (ongoing)

The context-help.pd file serves as a Table of Contents for all Context documentation.


LIST OF EXTERNAL LIBRARIES REQUIRED BY CONTEXT:

zexy
cyclone
else (1.0-beta8 or later)
flatgui
list-abs
hcs
iemguts (v 0.2.1 or later)
pddp (useful but not essential)
iemmatrix


LIST OF ALL EXTERNAL OBJECTS USED IN CONTEXT:

cyclone/accum
cyclone/append
cyclone/fromsymbol
cyclone/funnel
cyclone/iter
cyclone/lessthan~
cyclone/onebang
cyclone/prepend
cyclone/prepend
cyclone/substitute
cyclone/tanh
cyclone/togedge
cyclone/uzi
cyclone/zl
else/break
else/fromany
else/order
else/link
else/routeall
else/toany
else/window
flatgui/entry
hcs/canvas_name
hcs/sys_gui
iemguts/canvasargs
iemguts/canvasconnections
iemguts/canvasdelete
iemguts/canvasdollarzero
iemguts/canvaserror
iemguts/canvasindex
iemguts/canvasname
iemguts/canvasobjectposition
iemguts/canvasposition
iemguts/canvasselect
iemguts/classtest
iemguts/closebang
iemguts/oreceive
iemguts/propertybang
iemguts/receivecanvas
iemguts/savebangs
iemguts/sendcanvas
iemmatrix/matrix
iemmatrix/mtx_check
list-abs/list-drip
list-abs/list-extend
list-abs/list-filter
list-abs/list-map
list-abs/list-pad
list-abs/list-replace
zexy/demux
zexy/l2s
zexy/msgfile
zexy/mux
zexy/pack
zexy/relay
zexy/s2l
zexy/sort
zexy/time
zexy/unpack
zexy/urn



CREDITS:

Many people have contributed techical and moral support for Context. I would especially like to thank Miller Puckette, Alexander Torres Porres, Dan Wilcox and IOhannes Zmoelnig, Matt Barber and Derek Kwan for responding to many requests and bug fixes in PD and its external libraries, without which Context would not work. Omar Misa has provided consistent feedback and has the title of being Context's first User. And I would also like to thank Joe Deken and Ann Josey for their continued belief in me and in this project. Context certainly wouldn't be what it is without them.



Comments, feedback, suggestions, corrections and monologues are all welcome. Email liam.goodacre@gmail.com
