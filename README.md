EN

# Star-Rail-Model-Importer (SRMI)
Tools and instructions for importing custom models into Honkai Star Rail.

#### DISCLAIMER: I strongly recommend only using private servers for modding. Using these tools on official Star Rail servers carries a high risk of being banned. I do not condone the use of these tools and programs on official servers, and take no responsibility for any consequences as a result if you do. 

SRMI is a version of 3DMigoto/GIMI that I have modified to be compatible with Star Rail. Note that a lot of the files here have been ported over from GIMI and I am in the process of fixing them for Star Rail - many of them might have compatability issues and there may be a few references that still point to genshin resources.

 Feel free to use or modify any of the scripts on this repo as you wish, though please give credit if you use these programs in your projects. I am continuing to update this page with new features and fixes, so check back often.

Troubleshooting guide: [Troubleshooting](Guides/Troubleshooting.md)

Star Rail modding is still recent, so guides are still in progress. Many of the techniques are similar to GIMI, but for more help modding please visit the AGMG discord (https://discord.gg/agmg)

Model files for the importer are located at [SR-Model-Importer-Assets](https://github.com/SilentNightSound/SR-Model-Importer-Assets)

## Installation Instructions (3DMigoto)

1. Download a 3dmigoto .zip and extract it. I have provided two versions:
   - "3dmigoto-SRMI-for-development.zip" is a development version intended for creating mods which has all features turned on (including the green text at the top and bottom of the screen) but is slower
   - "3dmigoto-SRMI-for-playing-mods.zip" is a version of the program indended for playing mods which has development features turned off (no green text) but is faster

2. For loading 3dmigoto, run  `3DMigotoLoader.exe` as admin. Note that the exe has been compiled from python so Windows Defender might flag it - if you are having issues running the exe because it is being blocked, I have also provided `3DMigotoLoader.py` which has the same code (you will need to install the psutil and pyinjector dependencies to run it)

3. If everything is correct so far, 3DMigoto should be injected into the game and you should see a green text overlay (only if using the "for development" version, the "for playing" version does not show the green text):

4. Installation complete! You should now be able to load custom resources and override textures and shaders with 3DMigoto. To add mods, place them in the Mods folder (one mod per character at a time) and press F10 to load them in game:


&nbsp;
## Installation Instructions (3DMigoto Blender Plugin)

In order to modify game models, you need to also setup your Blender plugins and environment. The 3DMigoto plugin works with Blender 2.80+

NOTE! If using the GIMI plugin, please uninstall that version and use the SRMI plugin instead. They have almost the same functionality, but the SRMI plugin has an additional export option for Star Rail mods.

1. Download and install Blender

2. Download and install the modified 3DMigoto plugin (blender_3dmigoto_srmi.py) from [releases](https://github.com/SilentNightSound/SR-Model-Importer/releases). You can install an add-on in Blender by going to Edit -> Preferences -> Add-Ons -> Install, then selecting the .py file. 

3. If done correctly, you should see 3dmigoto in the plugin list as well as new options in the import and export menus

<img src="https://user-images.githubusercontent.com/107697535/174328624-ccb14ded-57b2-4ac7-b0a0-0de118119174.png" width="800"/>

<img src="https://user-images.githubusercontent.com/107697535/174329025-981a1a9f-7c56-4f44-804b-1b0394b8bd33.png" width="800"/>

&nbsp;
## Acknowledgements

Huge thank you to DarkStarSword, bo3b and Chiri for 3dmigoto!
