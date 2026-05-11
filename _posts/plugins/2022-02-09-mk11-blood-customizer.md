---
title: Blood Customizer
date: 2022-02-09 15:10:00 +0100
categories: [Modifications, Mortal Kombat 11]
tags: [pc, asi, mk11, mk]   
image: https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/mods/mk11/bc/1.jpg
description: Change blood color.
pin: false
hidden: false
---

# Introduction
A plugin for Mortal Kombat 11 which allows to change blood color for everyone.

<div class="alert bg-dark">
 Blood Customizer was only tested with latest Steam version!
</div>

<div class="alert bg-dark">
 There's 2 versions, standalone and MK11Hook plugin version.
</div>

<div class="alert bg-dark">
 BloodCustomizer only changes blood FX! Any character textures or FX (such as Skarlet's blood balls) won't be changed!
</div>

# Screenshots

<img class="img-fluid mx-auto" alt="1" src="{% link assets/mods/mk11/bc/1.jpg %}">
<img class="img-fluid mx-auto" alt="2" src="{% link assets/mods/mk11/bc/2.jpg %}">
<img class="img-fluid mx-auto" alt="3" src="{% link assets/mods/mk11/bc/3.jpg %}">
<img class="img-fluid mx-auto" alt="4" src="{% link assets/mods/mk11/bc/4.jpg %}">
<img class="img-fluid mx-auto" alt="4" src="{% link assets/mods/mk11/bc/5.jpg %}">

# Download

<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/MK11.BloodCustomizer/releases/latest/download/BloodCustomizer.zip" role="button">
<i class="fas fa-download"></i>
Download (Standalone)
</a>
<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/MK11.BloodCustomizer/releases/latest/download/BloodCustomizerEHP.zip" role="button">
<i class="fas fa-download"></i>
Download (MK11Hook Version)
</a>
<br>
<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/MK11.BloodCustomizer/" role="button">
<i class="fab fa-github"></i>
Source
</a>

# Installation 

## Standalone

Extract **BloodCustomizer.zip** to Binaries\Retail folder of Mortal Kombat 11.

If you are not sure how to find your Mortal Kombat 11 folder, search for it in your Steam library then right click on the entry and select Manage->Browse local files.

Archive breakdown:

 - dinput8.dll - [Ultimate ASI Loader](https://github.com/ThirteenAG/Ultimate-ASI-Loader/)
 - BloodCustomizer.asi 
 - BloodCustomizer.ini - configuration file


## Plugin version


Install <a href="https://ermaccer.github.io/posts/mk11hook/">MK11Hook</a>. Version 0.6.0 and higher is required.

Extract **BloodCustomizerEHP.zip** to Binaries\Retail folder of Mortal Kombat 11.

If you are not sure how to find your Mortal Kombat 11 folder, search for it in your Steam library then right click on the entry and select Manage->Browse local files.


Archive breakdown:

 - BloodCustomizer.ehp - mod itself
 - BloodCustomizer.ini - configuration file

Open up the MK11Hook menu and you will see a new plugins tab with Blood Customizer section which allows to tune colors during gameplay.



# Usage

If installed correctly, you will immediately notice blood color change. The default color is light blue.


# Configuration

BloodCustomizer can be configured using BloodCustomizer.ini file - you can open it with any text editor.

Each color value accepts values from 0 to 255.

Default is 0, 30, 140.

If using the MK11Hook version, you can configure colors visually in the added plugin tab.
