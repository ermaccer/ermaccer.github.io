---
title: Extra Weapons
date: 2021-12-24 21:57:00 +0200
categories: [Modifications, Manhunt]
tags: [pc, manhunt]   
img: https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/mods/mh/ew/1.jpg
short: Add weapons to Manhunt.
pin: false
---

# Introduction

Extra Weapons is a simple mod aiming to add "unique" weapons to Manhunt.


# Weapons

- Grenade

# Screenshots

![Preview](https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/mods/mh/ew/1.jpg)
![Preview](https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/mods/mh/ew/2.jpg)

<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://drive.google.com/file/d/1D9GYOE6vfFLhFiYVgvqrUNRqaIwVFo_P/view?usp=sharing" role="button" target ="_blank">
<i class="fas fa-download"></i>
Download
</a>


# Installation 

- Install [All weapons in all levels 2021](https://www.dixmor-hospital.com/mods/view/all-weapons-in-all-levels-2021)
- Set **bHookExtraWeapons** in PluginMH.ini to true.
- Extract everything to main Manhunt folder.



# Usage

Currently, added weapons can only be created using console or menu.

Find weapon entry in Entities section of the PluginMH (F2 opens by default) menu or use console to create new weapons.

eg.

`create Grenade_(CT)`

# Notes

- Thrown grenade will spin on the floor until it explodes - this is how it will need to work for now (the spinning is result of physics force not releasing on hit).
- Detonation countdown starts only if the grenade hit the floor.
