CONTEXT V3.0.2

Copyright Liam Goodacre, 2017-2018

This is a beta version of Context v3.0.2. There are still some bugs left and your help in tracking down both of these will be much appreciated.


SETUP:

Context runs on PD Vanilla V 0.47 or later. It needs the following externals, all available on Deken:

zexy
cyclone
moocow
flatgui
list-abs
hcs
iemguts (v 0.2.1 or later)
pddp (useful but not essential)
iemmatrix (only needed for [gridcontrol])


Once you have all the necessary externals, declare the main Context folder as a path (Edit --> Preferences --> Path --> New). You should also consider adding the text "-font-face normal" into the startup flags (Edit --> preferences --> Startup --> Startput Path). This fixes a bug in 0.47 where the text is bolded, which throws the float and symbol atom off in the main GUI. Hopefully this won't be necessary in later releases.

Context does not currently work on L2Ork or Purr Data.

Context patches sometimes take a long time to load (some of them several minutes). You can speed this up by turning off DSP before loading, then turning it back on. Faster machines are recommended.


TEXT SIZE

Different installations sometimes have different font sizes, which throws off the alignment of the float- and symbol-atoms on the Context GUI. You can (hopefully) fix this annoyance in the [config] file in the main folder. If the atoms are not perfectly conjoined, then open the config.pd file and change the connection from "bold" to "thin" or vice versa. I can't guarantee that this will accomodate every system though. If you're still having trouble, please report a bug.


DOCUMENTATION:

There are four parts to the Documentation:

1. The Context Manual. This is included in this folder as an odt and pdf. This is the most comprehensive guide of what Context is and how to use it.
2. Examples files, housed in the 'helpfiles' folder. These reference the manual and are meant to be studied in parallel with it.
3. Help prompts built into the Context menu. You can access these from within PD by right clicking on Context, selecting "properties" and clicking on the last item on every page (except the first one).
4. video tutorials at https://www.youtube.com/channel/UC_9u0n_ugUW7OjWrJRvhTjA (ongoing)

The context-help.pd file serves as a Table of Contents for all Context documentation.



Comments, feedback, suggestions, corrections and monologues are all welcome. Email liam.goodacre@gmail.com
