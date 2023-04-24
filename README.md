# QuakeLive Config Cleaner
Intended to clean up a single config file containing binds, vstrs, aliases, and cvars.

Identifies cvars that aren't recognized by quakelive and vstr that aren't called by binds. 

Logic could be improved to identify scripts called by other scripts. This version only looks at 1 level of depth (called by a bind directly). 

Comments out cvars related to server broadcast (MOTD etc), read-only cvars, and cheat-enabled only cvars. 

## Pre-requisites
1. Python >= 3.10 (available on Microsoft Store for easy download and installation)
## Installation
1. Download the main.py file to your computer

## Usage
1. Open the file with Python -> Right Click -> Open with
2. Choose the cfg file to process (uses the steam path to quakelive by default)
3. Save the processed cfg file (also uses the steam path to quakelive by default)
4. Optionally, in quakelive, run unbindall, unaliasall, cvar_restart
5. In quakelive, run exec your_saved_file.cfg
6. Optionally, in quakelive, run vid_restart, writeconfig autoexec.cfg
