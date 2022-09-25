---
title: SSFExplorer
date: 2021-04-25 22:30:00 +0200
categories: [Tools, Archives]
tags: [psp, mk, mku, unchained, ps2, mk, mkd, deception, mka, armageddon]  
image: https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/tools/ssf/ssf_explorer.jpg
description: Edit archives from classic PS2 era MK games!
hidden: false
---

![Preview](https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/tools/ssf/ssfexplorer.png)

SSFExplorer allows you to edit and view archives from classic PS2 era Mortal Kombat games.
It also has a texture exporter.


### Features
- Build & Extract archives from:
	- Mortal Kombat: Deception
	- Mortal Kombat: Armageddon
	- Mortal Kombat: Unchained
	- Mortal Kombat: Deadly Alliance
- Export textures from:
	- Mortal Kombat: Deception (PS2)
	- Mortal Kombat: Armageddon (PS2)
	- Mortal Kombat: Unchained (PSP)
	- Mortal Kombat: Deadly Alliance (PS2)
- Filenames for:
	- Mortal Kombat: Unchained (PSP)
	- Mortal Kombat: Armageddon (PS2) (INCOMPLETE)
- Extract MKDA.pak from PS2 games

Filenames were dumped from executable.




## Exporting Textures
It is recommended to use BMP + Alpha mass export option to build textures with alpha, alpha in TGA is not as smooth as combining
color BMP texture and alpha channel.


## Building Archive

To create an archive, you will need original file metadata -
this can be saved when you open any archive and select "Export For Building" option.

Open the ini file using File->Open INI.
This will load the configuration file and populate objects
in editing group.

If you want to create character archives (scorpion.sec for example), check "Build as character section file".
This option should be checked if FACEDAM file is present. This advice doesn't apply to MKDA.


## Download

<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/SSFExplorer/releases/latest/download/SSFExplorer.zip" role="button">
<i class="fas fa-download"></i>
Download
</a>
<br>
<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/SSFExplorer/" role="button">
<i class="fab fa-github"></i>
Source
</a>