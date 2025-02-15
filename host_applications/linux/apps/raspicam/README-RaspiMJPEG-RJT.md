# RJTidey Fork

Mar 5th 2015
Raspimjpeg support for separate settings for time-lapse
Raspimjpeg copy cam.jpg as thumbnails for captures

Mar 6th 2015
Raspimjpeg loading settings moved to a separate function and
made more tolerant of syntax / spacing. Config file can point to
a separate user config file which can overwrite values.

March 7th 2015
Config files are reloaded during startall operations so if stopped and started
they take effect
Command Pipe cleared out during start up.
Command processing moved to separate routine

March 8th 2015
Change thumbnail naming to append [vit]Number.th.jpg
This is used by preview to tie thumbnail to source irrespective of base naming

March 9th 2015
Naming scheme switched to using different letters for date fields and image counts
which may be put in any order
Add in annotation to same naming scheme

March 10th 2015
Removed command line switches to set image and video indexes
These are now automatically set within raspimjpeg by a directory scan

March 11th 2015
Fix for motion triggered time-lapse

March 18th 2015
Naming rules can now be used to create sub-folders under the base media path
Thumbnails are stored in the root media but have a flattened pathname to the main capture included

March 19th 2015
Added v3 annotation support

March 24th 2015
More tolerant error handling
Background boxing mode

April 3rd 2015
Config handling rewritten to use an enumerated set of config names and corresponding string and variables.
Now directly supports persisting changes to the user_config file.

April 4th 2015
Supports writing to a log file

April 5th 2015
Centralised status updates
Allowed image capture in video mode

April 9th 2015
Split up RaspiMJPEG over 4 files plus header
RaspiMJPEG.c main + config routines
RaspiMCam.c Camera access routines
RaspiMCmds.c Commands
RaspiMUtils.c General utilities
