---
title: BadBoys2Patch
date: 2024-11-21 20:00:00 +0100
categories: [Modifications, Bad Boys 2]
tags: [asi, pc, bad_boys]   
image: https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/mods/bb/patch/1.jpg
description: Crash fix and modern resolution support.
hidden: false
---

A patch for PC version of Bad Boys 2 (Miami Takedown)

<div class="alert bg-dark">
    This plugin was tested only with:
    <ul>
    <li>BBpc.exe - 3424323 bytes</li>
    <li>Launcher.exe - 1253376 bytes</li>
    </ul>
</div>

# Changelog
- Fixes "Error during Babel initialisation" error during startup on 4GB+ RAM systems
- Fixes 2D scaling for any selected resolution
- Adds all supported screen resolutions to the configuration launcher
- Adds an option to change FOV factor (bb2patch.ini)


# Screenshots
<img class="img-fluid mx-auto" alt="1" src="{% link assets/mods/bb/patch/1.jpg %}">
<img class="img-fluid mx-auto" alt="2" src="{% link assets/mods/bb/patch/2.jpg %}">

## Updated configuration launcher
<img class="img-fluid mx-auto" alt="2" src="{% link assets/mods/bb/patch/newLauncher.png %}">


# Download

<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/BadBoys2Patch/releases/latest/download/BadBoys2Patch.zip" role="button">
<i class="fas fa-download"></i>
Download
</a>
<br>
<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/BadBoys2Patch/" role="button">
<i class="fab fa-github"></i>
Source
</a>


# Installation 

Extract **BadBoys2Patch.zip** to root folder of Agent Hugo Hula Holiday.

Archive breakdown:

 - dsound.dll - [Ultimate ASI Loader](https://github.com/ThirteenAG/Ultimate-ASI-Loader/)
 - BadBoys2Patch.asi
 - bb2patch.ini