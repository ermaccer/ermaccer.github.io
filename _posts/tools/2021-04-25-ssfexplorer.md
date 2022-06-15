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
It also has a simple texture exporter.


### Features
- Build & Extract archives from:
	- Mortal Kombat: Deception
	- Mortal Kombat: Armageddon
	- Mortal Kombat: Unchained
- Extract archives from:
	- Mortal Kombat: Deadly Alliance
- Export textures from:
	- Mortal Kombat: Deception (PS2)
	- Mortal Kombat: Armageddon (PS2)
	- Mortal Kombat: Unchained (PSP)
- Filenames for:
	- Mortal Kombat: Unchained (PSP)

Filenames were dumped from executable.




## Exporting Textures
When exporting textures from PS2 games, you might see that they have invalid 
colors - this can be fixed by checking "Pal. Fix".


## Building Archive
**Building is supported for all games and platforms except MKDA!**


To create an archive, you will need original file metadata -
this can be saved when you open any archive and select "Export For Building" option.

Open the ini file using File->Open INI.
This will load the configuration file and populate objects
in editing group.

If you want to create character archives (scorpion.sec for example), check "Build as character section file".
This option should be checked if FACEDAM file is present.


## Download
[Download](https://github.com/ermaccer/SSFExplorer/releases/latest/download/SSFExplorer.zip)

