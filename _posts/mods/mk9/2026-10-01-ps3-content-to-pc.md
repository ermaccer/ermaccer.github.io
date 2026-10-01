---
title: PS3 Content
date: 2026-10-01 02:00:00 +0100
categories: [Modifications, Mortal Kombat Komplete Edition]
tags: [pc, asi, mk9, mk]   
image: https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/mods/mk9/ps32pc/1.jpg
description: Ports over Kratos and Chamber of the Flame stage to PC.
hidden: false
---

# Introduction
Ports over the PS3 Kratos character and Chamber of the Flame content to PC with added features.


<div class="alert bg-dark">
	Tested only tested with latest Steam version!
</div>

# Features
- Kratos and Fear Kratos (alt costume)
- Chamber of the Flame stage
- Input device aware QTE button prompts, keyboard will use generic prompts while controller will use X/Y/A/B or PS3 if picked (more below)
- Both Kratos and the stage can appear in randomized ladder
- Full nekropolis support
- Kratos specific fatalities


<div class="alert bg-dark">
	If you don't want Kratos specific fatalities, remove Character_Kratos_Fatality.xxx archives!
</div>

# Screenshots
<img class="img-fluid mx-auto" alt="1" src="{% link assets/mods/mk9/ps32pc/1.jpg %}">
<img class="img-fluid mx-auto" alt="1" src="{% link assets/mods/mk9/ps32pc/9.jpg %}">
<img class="img-fluid mx-auto" alt="1" src="{% link assets/mods/mk9/ps32pc/2.jpg %}">
<img class="img-fluid mx-auto" alt="1" src="{% link assets/mods/mk9/ps32pc/6.jpg %}">
<img class="img-fluid mx-auto" alt="1" src="{% link assets/mods/mk9/ps32pc/5.jpg %}">
<img class="img-fluid mx-auto" alt="1" src="{% link assets/mods/mk9/ps32pc/8.jpg %}">
<img class="img-fluid mx-auto" alt="1" src="{% link assets/mods/mk9/ps32pc/10.jpg %}">

# Download

<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://mega.nz/file/cI5DQajY#3ZA2by_Hc9PVDOIh5_KB3qwEdUUip0Mz9qr-IRglDxI" role="button">
<i class="fas fa-download"></i>
Download
</a>

# Installation 

Extract **PS3ContentToPC.zip** anywhere.

Copy the contents of `PS3Content` to DiscContentPC folder of Mortal Kombat 9. Make sure that `dinput8.dll` and `MK9Addon.asi` are near `MKKE.exe`. Confirm overwrite.

Kratos will be added to the DLC select after Cyber Sub-Zero and stage will be also available in arena select screen.


Archive breakdown:

 - dinput8.dll - [Ultimate ASI Loader](https://github.com/ThirteenAG/Ultimate-ASI-Loader/)
 - MK9Addon.asi - [MK9Addon](https://github.com/ermaccer/MK9Addon)

Bundled MK9Addon is pre-configured to include Chamber of the Flame stage.


# Extra Scripts

There's a few optional scripts to change some things. They are in Extra folder, to use them, pick one and copy it to `MKScript` folder, overwriting existing one.

| Script | Description |
| --- | --- |
|ChamberOfFlameNoShake|  Removes camera shaking whenever background changes appear (statue, Gaia breakthrough). |
|ChamberOfFlamePS3IconsNoShake|  Removes camera shaking whenever background changes appear (statue, Gaia breakthrough). Replaces XBOX prompts with original PS3 ones.|
|ChamberOfFlamePS3Icons| Replaces XBOX prompts with original PS3 ones.|
|KratosPS3Icons| Replaces Kratos QTE XBOX prompts with original PS3 ones.|


