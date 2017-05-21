CONTEXT V3.0.1

RELEASE DATE: 19th April, 2017

This is a beta version of Context v3.0.1 for testing purposes. There are many bugs in the software and many holes in the documentation. Your help in tracking down both of these will be much appreciated.


SETUP:

Context runs on PD Vanilla V 0.47 or later. It needs the following externals, all available on Deken:

zexy
cyclone (v 0.0.extended) *
moocow
flatgui
list-abs
iemguts (v 0.2.1 or later)

* Hopefully the new Cyclone releases will be compatible soon. 

Once you have all the necessary externals, declare the main Context folder as a path (Edit --> Preferences --> Path --> New). You should also consider adding the text "-font-face normal" into the startup flags (Edit --> preferences --> Startup --> Startput Path). This fixes a bug in 0.47 where the text is bolded, which throws the float and symbol atom off in the main GUI. Hopefully this won't be necessary in later releases.

Context does not currently work on L2Ork or Purr Data.

Context patches sometimes take a long time to load (some of them several minutes). You can speed this up by turning off DSP before loading, then turning it back on. Faster machines are recommended.


DOCUMENTATION:

There are four parts to the Documentation:

1. The Context Manual. This is included in this folder as an odt and pdf. This is the most comprehensive guide of what Context is and how to use it.
2. Examples files, housed in the 'helpfiles' folder. These reference the manual and are meant to be studied in parallel with it.
3. Help prompts built into the Context menu. You can access these from within PD by right clicking on Context, selecting "properties" and clicking on the last item on every page (except the first one).
4. *-help.pd files. Quite underdeveloped at this point.
(5. Forthcoming: video tutorials).



Comments, feedback, suggestions, corrections and monologues are all welcome. Email liam.goodacre@gmail.com
