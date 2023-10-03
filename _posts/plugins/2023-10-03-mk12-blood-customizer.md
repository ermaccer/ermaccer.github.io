---
title: Blood Customizer
date: 2023-10-03 19:01:00 +0100
categories: [Modifications, Mortal Kombat 1]
tags: [pc, asi, mk1, mk, imgui]   
image: https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/mods/mk1/bc/1.jpg
description: Change blood color.
pin: false
hidden: false
---

# Introduction
A plugin for Mortal Kombat 1 which allows to change blood color for everyone.

<div class="alert bg-dark">
 Blood Customizer was only tested with latest Steam version!
</div>

<div class="alert bg-dark">
 There's 2 versions, standalone and MK1Hook plugin version which allows to use both mods at once.
</div>

# Features
- Set any RGB for all blood effects (fatality textures have colored overlays)
- Two levels of color brightness

# Screenshots
<img class="img-fluid mx-auto" alt="1" src="{% link assets/mods/mk1/bc/1.jpg %}">
<img class="img-fluid mx-auto" alt="2" src="{% link assets/mods/mk1/bc/2.jpg %}">
<img class="img-fluid mx-auto" alt="3" src="{% link assets/mods/mk1/bc/3.jpg %}">
<img class="img-fluid mx-auto" alt="4" src="{% link assets/mods/mk1/bc/4.jpg %}">

# Download

<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/MK1.BloodCustomizer/releases/latest/download/BloodCustomizer.zip" role="button">
<i class="fas fa-download"></i>
Download (Standalone)
</a>
<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/MK1.BloodCustomizer/releases/latest/download/BloodCustomizerEHP.zip" role="button">
<i class="fas fa-download"></i>
Download (MK1Hook Version)
</a>
<br>
<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/MK1.BloodCustomizer/" role="button">
<i class="fab fa-github"></i>
Source
</a>


# Installation 

## Standalone

Extract **BloodCustomizer.zip** to MK12\Binaries\Win64 folder of Mortal Kombat 1 (so that **dsound.dll** ends up near **SDL2.dll**).

If you are not sure how to find your Mortal Kombat 1 folder, search for it in your Steam library then right click on the entry and select Manage->Browse local files.

Archive breakdown:

 - dsound.dll - mod itself
 - BloodCustomizer.ini - configuration file


## Plugin version


Install <a href="https://ermaccer.github.io/posts/mk1hook/">MK1Hook</a>. Version 0.3 and higher is required.

Extract **BloodCustomizerEHP.zip** to MK12\Binaries\Win64 folder of Mortal Kombat 1 (so that **MK1.BloodCustomizer.ehp** ends up near **SDL2.dll**).

If you are not sure how to find your Mortal Kombat 1 folder, search for it in your Steam library then right click on the entry and select Manage->Browse local files.

Archive breakdown:

 - MK1.BloodCustomizer.ehp - mod itself
 - BloodCustomizer.ini - configuration file

Open up the MK1Hook menu and you will see a new plugins tab with Blood Customizer section which allows to tune colors during gameplay.



# Usage

If installed correctly, you will immediately notice blood color change. The default color is dark green.


# Configuration

BloodCustomizer can be configured using BloodCustomizer.ini file - you can open it with any text editor.

Each color value accepts values from 0 to 255.


