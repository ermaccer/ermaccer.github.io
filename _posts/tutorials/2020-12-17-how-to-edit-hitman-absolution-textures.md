---
title: How To Edit Hitman Absolution Textures
date: 2020-12-17 17:03:00 +0200
categories: [Help, Guides]
tags: [hitman, absolution, textures, mod, modding, swap]   
description: A simple guide on how to replace textures in Hitman Absolution.
hidden: true
---

## Introduction
This guide requires you to have minimum hex editing skills.
Designed to edit 47's suits.

### Requirements
- Hex editor, I recommend HxD for simple stuff like this
[Download](https://mh-nexus.de/en/downloads.php?product=HxD20)
- Hitman Absolution extracting tool (hitman5.rar archive - I'm not sure if I can reupload)
[Download](https://forum.xentax.com/viewtopic.php?f=16&t=15883)

## Guide
Files were edited in GOG version - packages are most likely
different in other releases.

**This covers DDS editing only - TGA textures are a bit harder**

Quick reference:
66F39003B60F42EFE5F4555F3DDFAAF6 - Default suit with earpiece (used in first mission)

### Extracting 47 packages
You will need to find "hitmanmodels.template" inside
runtime->templates->characters->hitman->outfits.

Extract extracting tools there.

Your directory should look like this.

Drag any suit package (with .pc_resourcelib extension) onto Hitman5.exe.


The package is extracted to a folder with package filename.

![Preview](https://github.com/ermaccer/ermaccer.github.io/blob/gh-pages/assets/tutorials/abso-te/folder.png?raw=true)

We are interested in the .TEXT files - textures.
Place Hitman5dds.exe in this folder and run it.

You should get multiple .dds and .tga files.

Check which texture looks like some part suit and remember copy it - this will
be our new texture to replace.

For example, 003A.dds is the pants texture in our file.

Copy it to something like newpants.dds. You need to edit the copy, not original
as we need original file in order to place it back inside the archive.

Edit your copied texture.

# Editing texture in package
Open original texture with HxD, note down DXT version (your new one needs to be the same) then delete first 128 bytes (Length - 0x80);
Hit CTRL+A and write length somewhere - you'll need it.

A file with stripped header:
![Preview](https://github.com/ermaccer/ermaccer.github.io/blob/gh-pages/assets/tutorials/abso-te/after.png?raw=true)



Open original package (.pc_resourcelib file) in a new HxD tab, go back to original texture tab.
Select some bytes from the beginning (100-200) and copy them to clipboard (CTRL+C).

In package tab, hit CTRL+F and choose Hex-values in Datatype with direction set to All.
Copy paste your previously copied bytes.

You should find your texture place - select the first value.
Right click on it and choose "Select block".

Type previously stored length of original texture.

Now a huge block of data should be highlited, don't do anything with it yet.


**Make sure you are in insert and not overwrite mode - press Insert to toggle**

Open your modded texture, remove first 128 bytes, select everything and copy.
Go back to archive tab, hit delete and then paste (CTRL+V).

Save the archive and you are all done.

# Releasing mods

Apparently each Absolution release uses different header values, to release your
mod you will most likely need to upload whole hitmanmodels.template folder.

# Examples

![Preview](https://github.com/ermaccer/ermaccer.github.io/blob/gh-pages/assets/tutorials/abso-te/example1.png?raw=true)

<iframe width="560" height="315" src="https://www.youtube.com/embed/yV2XMTXv0rk" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

