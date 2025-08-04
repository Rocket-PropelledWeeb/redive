---
title: Adding New Song Entries
---
# Adding New Song Entries

## What will this guide cover?

This guide will cover how to add a new song entry, jacket, charts, and audio to the game. It will also cover how to add infernos of existing entries. It will not cover music videos yet, perhaps in the future.

### What you'll need

- A working installation of the game. This has not been tested on versions other than 3.07.01 and 3.10, your mileage may vary on other versions.

- [UAssetGUI](https://github.com/atenfyr/UAssetGUI) (A generally useful tool for editing anything in Unreal Engine tables)

- [WSongInject](https://github.com/yellowberryHN/WSongInject) (This automatically handles all the metadata and jacket for your new song so you don't have to do it manually)

- [wacca-acb-editor](https://github.com/Raymonf/wacca-acb-editor) (This injects the audio into the game files)

- [MercuryTools](https://github.com/Yasu3D/MercuryTools) (Optional, but makes editing the tables much easier)

- A text editor, preferably with syntax highlighting. I recommend [Notepad++](https://notepad-plus-plus.org/downloads/)

----
## Adding a new song

### Step 1: Adding your audio

wacca-acb-editor todo  
make sure to edit the batch file for 3.10



--- 
### Step 2: Adding your song entry

Open WSongInject and select the game directory containing WindowsNoEditor. Set your ID to the one corresponding to your song output by the acb editor.

From here, you can fill in all the fields. Change the level of the inferno to automatically make an inferno entry as well. Set to 0 if you don't want to have an inferno for your song. 

Once the fields are filled out, click the "Inject" button on the bottom. **This will only work once, so make sure your information is correct!** We can edit the data later if needed with other tools, but it'll be much less convenient.

Your jacket can be created via the button on the bottom at any time. Unlike the metadata, this can be repeated and will overwrite any previous files.

---
### Step 3: Adding your charts

Make a folder in ``<insert path here>`` with the name of the ID of your chart. Use the other charts as examples. (Example: ID 4001 would be ``S04-001``)

Copy your .mer files into this folder and rename them. The format is the same as the folder, plus ``_xx`` at the end for their corresponding difficulty. ``00`` for normal, ``01`` for hard, ``02`` for expert, and ``03`` for inferno. (Example: ID 4001's expert chart would be renamed to ``S04-001_02``)

After this, open each mer file and append the MER_BGM ID from the wacca-acb-editor output list to the ``#MUSIC_FILE_PATH`` line. (Example: ID 4001 should look like ``#MUSIC_FILE_PATH MER_BGM_S04_001``). Make sure you save the file before closing your editor.

That's it! Your song should appear in game!

---
## Adding infernos for existing entries
This can be a bit more tricky than a new entry. This section will cover both the manual method and the method via MercuryTools


---
### Using MercuryTools

todo later easy guide need to grab screenshots

---
### The Manual Method

todo not as easy guide need to grab screenshots

---
## Troubleshooting & Editing

Some time in live, everything pencil and everything smoothly with pencil is going smoothly. But then, unexpected happening it is happening unexpectedly in life. The importance thing to do is to make solution to the problem so problem is solutioned problem solution problem. Chair. 

### MercuryTools

MusicParameterTable editing in MercuryTools is easy! Woo!

### UAssetGui

Not quite as easy. Boo! But, not that hard either.