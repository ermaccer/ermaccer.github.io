---
title: How To Install Mortal Kombat PS2 Mods
date: 2020-12-28 20:45:00 +0200
categories: [Help, Guides]
tags: [ps2, iso, mk, mkd, mka, deception, armageddon]
description: Learn how to install most of my PS2 MK mods.
hidden: false
---

## Introduction
This guide requires you to have knowledge of PS2 ISO rebuilding,
it does not cover it.
A great tutorial on how to do that can be found [here](https://www.obscuregamers.com/threads/how-to-create-a-working-playstation-2-master-cd-r-or-dvd-r-image.772/)



### Requirements
- Game ISO


## Guide

### Extracting ISO
You will need to extract your game ISO.

**Using built-in Windows 10 functionality**

If you use Windows 10, you should be able to open ISO contents by just
double clicking at the .ISO file.

![Preview](https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/tutorials/mk_d_a-ps2tut/explorer.png)

Select both items and drag them over to a folder (create new or existing one).

## Preparing game data
Create a new folder somewhere, copy MKDA.PAK and game executable (SLXX_YYY.YY file)
to this folder from extracted game directory.

Place all files from mod archive here.

## Installing

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
