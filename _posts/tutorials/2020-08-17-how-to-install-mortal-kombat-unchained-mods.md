---
title: How To Install Mortal Kombat Unchained Mods
date: 2020-08-17 18:54:00 +0200
categories: [Help, Guides]
tags: [psp, iso, mk, mku, unchained]   
description: Learn how to install most of my MKU mods.
hidden: false
---

## Introduction
This guide is not meant for installing PPSSPP texture swaps (people commonly
reference them as mods), it is meant for installing mods which actually edit
the game files so you can use them on your real console or just play them
using any emulator.

### Requirements
- UMDGen (optional and if you plan to rebuild the iso) 
[Download](https://www.romhacking.net/utilities/1218/)

- Game ISO


## Guide

### Extracting ISO
You will need to extract your game ISO.

### Methods

**Using built-in Windows 10 functionality**

If you use Windows 10, you should be able to open ISO contents by just
double clicking at the .ISO file.

![Preview](https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/img/mkutut/exploreriso.png)

Select both items and drag them over to a folder (create new or existing one).

**Using UMDGen**

Download and extract UMDGen.

Run the program, open your game ISO and extract contents to a folder.

![Preview](https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/img/mkutut/umdgeniso.png)



## Preparing game data

Open **PSP_GAME** folder, go to **SYSDIR** directory and delete/rename **EBOOT.BIN**.

Copy **BOOT.BIN** from the same directory, rename it as **EBOOT.BIN**.

This step replaces encrypted PSP executable with a clean one.


## Installing Mods
Download any mod, extract archive contents to **PSP_GAME** directory.

Your game folder should look like this:

![Preview](https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/img/mkutut/modsiso.png)

Execute Install-GAMEREGION.bat to install the mod.

If you don't know what ULES and ULUS mean:

**ULES** - European Release

**ULUS** - United States Release

***NOTE: Selecting wrong installer might break your game and you will need to start over, please be careful!***


All done, now you can navigate to your modded folder in PPSSPP to play the game without the need of an ISO.

Feel free to remove mod files after installing one.

## Rebuilding ISO

If you want to run mods on real hardware (or don't want to play the game from a folder) , you will need to rebuild/edit the ISO.

Launch UMDGen again, open your ISO and do the following:
 - Drag EBOOT.BIN from your modded copy folder to PSP_GAME\SYSDIR folder in UMDGen, confirm overwrite
 - Drag ARCHIVE.BIN/ARCHIVE.IMP from your modded copy folder to PSP_GAME\USRDIR in UMDGen, confirm overwrite
 
Once this is done, select File->Save As and save your new ISO somewhere.

***NOTE: Please use Save As option whenever you are doing ISO changes, Save option might sometimes break the file***



