# Repository Content
This repository contains ViRMEn, the Virtual Reality MATLAB Engine. Various versions are archived as zip files in the `Software` folder. The VR design is documented in the `VR design` folder. 

# Version History

2011-04-11
- First version of ViRMEn (not available on Webspace)

2013-02-27
- First version released on Webspace

2013-06-04
- Fixed warning about rendering in the texture refining window
- Corrected vr.worlds{#}.objects.edges matrix bug

2013-11-21
- Updated the manual troubleshooting section

2014-07-09
- Improved GUI for importing textures/objects. GUI now displays a smaller number of items on multiple pages and allows switching between pages
- Added a new feature in the GUI: a toggle button for turning on/off transparencies in the current world. Turning off transparencies when they are not necessary improves the speed of graphics.
- Fixed the bug in which the ViRMEn GUI disappeared whenever an unexpected crash happened (and reappeared with two menu bars when >> virmen was run at the command line). Running >> virmen will now make the missing GUI visible.
- Corrected some errors and typos in the manual
- Fixed the automatic "Update ViRMEn" feature

2014-11-09
- MAJOR UPDATE with new and improved ViRMEn graphics engine
- Much faster engine (allows up to hundreds of thousands of triangles)
- Compatible with all Matlab versions from 2010 to 2014a
- Compatible with Mac OS
- New feature: window manager for outputting graphics to multiple monitors and/or windows
- Different monitors and/or windows can now use different transformation functions
- Full support for using image files as textures

2015-01-17
- MATLAB 2014b compatibility: fixed the bug that caused crashing on startup

2015-03-19
- MATLAB 2014b compatibility: fixed a number of bugs; ViRMEn should now be fully compatible with 2014b
- Took care of GUI speed problems that were being caused by the new graphics system in 2014b
- Fixed a bug that caused crashing when the user pressed "cancel" upon entering a new variable value
- Symbolic expressions now remain symbolic (rather than being converted to numberic values) when object or shape locations are added, deleted, or modified, including by drag-and-dropping
- Creating a warning system for when files are overwritten by built-in functions
- Fixed a bug that created glitches for velocity types of input devices that provide position, rather than velocity signals

2015-04-14
- Improved collision detection code to handle tight spaces like narrow corridors (see the new variable vr.dpResolution)
- Corrected a bug that caused ViRMEn not to start a second time after closing
- Corrected calculations, such that values of vr.dt across all iterations add up exactly to vr.elapsedTime, without depending on the precision of the computer clock
- Corrected a multi-window/monitor bug that prevented world background color to be updated properly in all windows
- Prevented crashing if the user specifies a monitor number that doesn't exist - the main monitor is now used instead

2015-10-05
- Added the option to allow the user-defined movement function to specify displacement or position instead of velocity

2016-02-12
- Fixed bugs related to 32-bit Matlab (some files were inadvertently omitted from the previous two versions)
- Fixed compatibility issues for Matlab 2015b