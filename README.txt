SB3 to SB2 Converter
A simple Python 3 program that converts .sb3 files to .sb2 files

Requirements
Python 3 (preferably 3.6.2 or later)
Installation
Download and extract the ZIP file and move the sb3tosb2.py file to wherever you want.

Usage
Run sb3tosb2.py with Python
Select the SB3 file to open
Either select the SB2 file to save to or type in a new file name
Click OK to exit
Usage (command line)
Open the terminal or command prompt and navigate to the directory of the sb3tosb2.py file.
Enter the following command: python sb3tosb2.py [unordered options] sb3path sb2path
Options are not necessary.
If an error is given, make sure you entered a valid sb3 file.
Arguments
Options should be separated by a space.
List of options:

-h: Displays the program arguments and list of options
-c: This enables compatibility mode. Workarounds for the following blocks will be added to sprites:
costume [number v]
set drag mode [ v]
<[] contains []?> (may result in performance loss)
(item # of [] in [ v]) (may result in performance loss)
pen color blocks (including HSV and shade blocks)
timer blocks
-j: Automatically enables compatibility mode and adds an unlimited join workaround (may result in significant performance loss)
-l: Automatically enables compatibility mode and adds custom blocks to automatically limit list length to 200,000 (may result in performance loss)
-p: Tries to insert blocks to fill the screen when the pen size is set to a value greater than 255
Known Issues
MP3 audio files cannot be converted
Compatibility mode changes variable monitor labels
Compatibility mode allows ([ v] of [ v]) to access only variables (not attributes like x position, backdrop #, etc.)
Dragging in projects converted with compatibility mode does not have the same pen behavior as in 3.0
Unlimited join does not check case when checking string equality