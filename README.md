# 3D-printer-Cura-profiles
Repository to hold the OctoPi Cura profiles for the Ipswich Makerspace 3D printers.

## Using the in-built Cura profiles
Octoprint has a plugin architecture, one plugin installed is the Cura plugin. This allows Cura .ini files (which detail how the slicing is to carried out) to be uploaded and applied to .stl files allowing slicing to be carried out locally on the Pi from an stl file without needing to do the slicing separately.

The Cura profiles have been named in such a way that they describe the slicer settings.

The file name is made up in several pieces as shown below.

Printer name | Fillament material | Hotend temperature | Infill percentage | Support settings | Platform settings

An example file name is:

`K8200_PLA_190_i30_s0_p0`

This translates as follows;

* `K8200` - The printer name
* `PLA` - The fillament type
* `190` - Hotend termperature of 190 degrees C
* `i30` - Infill at 30 %
* `s0` - No supports
* `p0` - No platform

the full range of options for supports are:

* `s0` - No supports
* `s1` - Support where touching Build plate
* `s2` - Support everywhere

the full range of platform options are:

* `p0` - No platform
* `p1` - Print with brim
* `p2` - Print with raft

## Creating your own profiles
Firstly, it may not be necessary to create your own profile, if you have some requirements that are not catered for by the profiles already provided, then you can slice your own 3D files using your own slicer of choice and then uploading the gcode produced directly into Octoprint. this eliminates the need to slice within Octoprint.

However, if you think the slicing profiles could be supplemented then feel free to create your own, but please use the file name convention shown above.

Unfortunately the Octoprint Cura plugin is a bit picky about which Cura .ini files it accepts. If you want to create a Cura profile you must download Cura version 15.04 or earlier. the newer version will not work. Cura can be downloaded here, please note version 2.x.x is actually newer than 15.x.x, the newer 2.x.x will not work.

NFire delta printer profile to be added.
