####################
#                  #
#  CONTEXT (v4.0)  #
#                  #
####################      Copyright Liam Goodacre, 2015-2018


RELEASE:

This is a general release of Context v4.0. It runs on PD Vanilla 0.48.1 or higher. It is compatible with Linux, OS and Windows. There are probably still some bugs left.


SETUP:

Once you have downloaded Context, you must declare its location so that PD knows how to find it on your computer. To do this, go to Edit --> Preferences --> Path --> New and select the location of Context's home folder.


EXTERNALS:

Externals are PD objects that are not available in PD Vanilla and must be installed seperately (Help --> Find Externals). Context relies heavily on externals (see LIST OF EXTERNAL LIBRARIES below). To make setup at easy as possible, Context distributes with all its external dependencies, according to the terms of their various licenses. This means that Context should work "out of the box" without the user having to manually download and declare external libraries. (Note: this only works for 64-bit systems; 32-bit users will have to provide their own externals).

There are some reasons why you might not want to use the externals which are distributed with Context. For instance, you might find that your patches are reverting to an unwanted version of an external object, if you have a different version of a library that the one Context is using. If you want to avoid the externals that are distributed with Context, or if you find that they are not working, simply delete or rename the following folders from the main Context folder: "cyclone", "else", "flatgui", "hcs", "iemguts", "iemmatrix" "list-abs", and "zexy". (Do not delete "ctxfiles" or "helpfiles"!) Context will now look for its external objects in your usual search directories, so make sure that your libraries are in order inside your "PD Documents Directory" or in another search path.


CONFIGURATION:

Context does not currently work on L2Ork or Purr Data. There is a patch called "config-distro.pd" that one day will hopefully be used to switch between the two distributions. For now, leave it set to Vanilla.

Different installations sometimes have different font sizes, which throws off the alignment of the float- and symbol-atoms on the Context GUI. You can fix this annoyance in the config-textsize.pd file in the main folder. Use the number boxes to move the red canvases until they coincide exactly with the symbol atoms, then save the patch.

Context has limited compatibility with Vanilla 0.47. If you want to run Context in 0.47, you can try replacing the file ctxfiles/dv.pd with ctxfiles/dv-047.pd, although this does not guarantee full functionality.

Context patches sometimes take a long time to load (some of them several minutes). You can speed this up by turning off DSP before loading, then turning it back on. Faster machines are recommended.


SYSTEM REQUIREMENTS:

The beauty of a modular system is that its weight depends on the way it is used in the patch, so Context should run on slower systems. That being said, Context is a heavy abstraction, and you should use it with some consideration for your system's resources.

Each instance of Context consumes about 6.65MB of RAM, and you can add 0.1MB per extra unit as Context is resized. On a very slow machine (1GHZ, 2GB) you can run about 15-20 instances of Context before it starts to seize up. On a faster machine (2.5GHZ, 4GB) you can safely run several hundred instances of Context without suffering audio glitches, although this will consume a lot of memory.

Unfortunately, creating, resizing and labeling Context will always cause audio dropouts.


DOCUMENTATION:

There are four parts to the Documentation:

1. The Context Manual. This is included in this folder as an odt and pdf. This is the most comprehensive guide of what Context is and how to use it.

2. Examples files, housed in the 'helpfiles' folder. These reference the manual and are meant to be studied in parallel with it.

3. Help prompts built into the Context menu. You can access these from within PD by right clicking on Context, selecting "properties" and clicking on the last item on every page (except the first one).

4. video tutorials at https://www.youtube.com/channel/UC_9u0n_ugUW7OjWrJRvhTjA (ongoing)

The context-help.pd file serves as a Table of Contents for all Context documentation.

Context website: https://contextsequencer.wordpress.com/
Facebook page: https://www.facebook.com/groups/123031095094961/


LIST OF EXTERNAL LIBRARIES REQUIRED BY CONTEXT:


zexy
cyclone
else (1.0-beta9 or later)
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
else/dir
else/fromany
else/openfile
else/order
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

Context is created and maintained by Liam Goodacre, but many people have contributed techical and moral support over the years. I would especially like to thank Miller Puckette, Alexander Torres Porres, Dan Wilcox, IOhannes Zmoelnig, Lucas Cordiviola, Roman Haefeli, Matt Barber and Derek Kwan for responding to many requests and bug fixes in PD and its external libraries. Without their help, Context would not work. Omar Misa has provided consistent feedback and has the title of being Context's First User, giving me the motivation needed to finish the project. Zack Lee has helped me improve Context's compatibility with externals, and Joshua Walker and Vassilis Poulantzas have provided a great deal of help with the documentation. Finally, I would also like to thank Joe Deken and Ann Josey for their continued belief in me and in this project. Context certainly wouldn't be what it is without them.

Comments, feedback, suggestions, corrections and monologues are all welcome. Email liam.goodacre@gmail.com


LICENSE:

Context is distributed under the GPL V3. See LICENSE.txt
