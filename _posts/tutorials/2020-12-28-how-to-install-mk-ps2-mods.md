---
title: How To Install Mortal Kombat PS2 Mods
date: 2020-12-28 20:45:00 +0200
categories: [Help, Guides]
tags: [ps2, iso, mk, mkd, mka, deception, armageddon]
description: Learn how to install most of my PS2 MK mods.
hidden: false
---


# Requirements
- **PS2 Tools** (cdvdgen, iml2iso) [Download](https://mega.nz/file/lURTjBYL#cWe9ZIOVIfD5nmwfimwx632Sz-fn1E1DpZddcF9RjJs)
- **PAK Tool** [Download](https://github.com/ermaccer/MortalKombat.PAKTool/releases/)

# Step by Step

## 1. Extracting ISO
If you use Windows 10 or newer, you should be able to open ISO contents by just
double clicking at the .ISO file. This will mount the ISO as a virtual drive.

Open up the newly mounted drive and simply move everything from the virtual drive to any folder (preferably create one just for UMKD stuff).


## 2. Replacing Files
Copy **MKDA.PAK** near PAKTool.exe, drag it onto the executable and wait until it is extracted.

Replace any files in the ps2dvd\art folder!

Once replaced, drag the ps2dvd folder back onto the executable, wait till it finishes then rename **ps2dvd.PAK** to **MKDA.PAK**.


## 3. Building a new  ISO

Open "cdvdgen", it's a tool designed to create PS2 DVD and CD images from scratch, it CANNOT edit existing ones!

### CDVDGEN Steps
1. Once launched, select **Create new project**
2. Select **DVD-ROM Master Disc**
3. Go to **Volume tab**
4. Once in volume tab, fill the respective places with following data, change SLUS (SLES) serial to match the game 
   - Master Disc/Disc name: **SLUS XXXXX**
   - Master Disc/Producer Name and copyright holder: **MIDWAY**
   - Master Disc/License Area: **America** or **Europe**
   - Volume Identifier/Volume: **SLUS-XXXXX**
5. Go to **Directory** tab
6. Start dragging files from your previously extracted folder onto this window. Make sure they end up in following order/hierarchy:
   - SYSTEM.CNF
   - NETR.OVL
   - NTGUI.ELF
   - SLUS_XXX.XX 
   - AREA51 (folder, can also be removed)
   - CNF (folder)
   - LICENSE (folder)
   - MODULES (folder)
   - MOVIEPS2 (folder)
   - NETGUI (folder)
   - SNDSPS2 (folder)
   - GAMER.OVL
   - LOADINGE.RAW
   - MKDA.PAK
   - MOVIER.OVL
7. Open **ASSETS** folder of UMKD.
8. In CDVDGEN **Directory** window, highlight **MKDA.PAK** and press delete or remove it using mouse
9. Drag newly built **MKDA.PAK** onto the **Directory** window
10. Save the project with File->Save, keep it around in case you'd like to install more mods and save some time
11. Choose **Export iml file** from File menu and save it somewhere you can find
12. Close CDVDGEN


Now open "iml2iso", it's a tool designed to convert the IML file listing into a working PS2 iso.

### IML2ISO Steps
1. Once launched, click the **...** button near IML file path
2. Locate your previously exported **IML** file from CDVDGEN and open it
3. Press **Start**
4. Wait till the ISO generation process is finished, the resulting .ISO file will be stored in the same path as selected .IML
5. Done



# Installing (old)
## This section is for old mods that have .bat files!

### Preparing game data
Create a new folder somewhere, copy MKDA.PAK and game executable (SLXX_YYY.YY file)
to this folder from extracted game directory.

Place all files from mod archive here.



Run **PatchSLXX.bat** to patch the executable (make sure region is correct!).

Run **ExtractPAK.bat** to extract MKDA.pak file. 
This will extract the archive to the **root** of your current drive, so 
contents end up in X:\ps2dvd (X being drive letter).

Go to the extracted folder and replace files in art folder with the ones from the 
mod.

After you have done that, run **BuildPAK.bat**.
An archive will appear in the root directory (ps2dvd.pak), rename it
to MKDA.PAK and copy it to the modified files folder.

Move MKDA.PAK and executable file back to original game folder.

Build a new ISO from the folder (guide linked in introduction).

Once that is done, you can either play the modified iso on a real console
or using an emulator.
