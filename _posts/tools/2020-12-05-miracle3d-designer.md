---
title: Miracle3D Designer
date: 2020-12-05 13:21:00 +0200
categories: [Tools, Model Editing]
tags: [m3d, battle_mages, sign_of_darkness, sod, bm, bmsod, miracle3d, sam, gsm]  
image: https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/tools/m3d/m3d_designer.jpg
short: Convert and edit Battle Mages models.
pin: false
---

![Preview](https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/tools/m3d/Designer.png)

Miracle3D Designer allows you to work with models used by Miracle3D engine - SAM
and GSM. They are used in Battle Mages and its addon Sign Of Darkness.


### Features
- Open SAM/GSM files
- Export to SMD and OBJ
- Supports Skeleton
- Supports Rigging Data
- Experimental Model Optimiztaion feature
- Decompile and Compile Models
- Export Animations to SMD




### Usage

## Exporting Model 

To simply convert SAM/GSM into SMD or OBJ, open any file (File->Open->Model) and select
Export->SMD or OBJ option to save the file in desired format.

## Decompiling Model 

You need to decompile a model before you can edit it. Open any model
using File->Open->Model then press "Decompile" button and specify folder where
it will be decompiled.

Decompilation will generate few files:

- model.ini 		<- Configuration of the model
- animationData.bin <- Binary animation data
- name.smd 			<- Model

As of 0.9, all animations are dumped to respective NAME.SMD files.
Importing is not supported yet.


You can only extract SMD files while decompiling.


## Compiling

To compile a model, you need to use a .ini file that can be obtained
by decompiling. Open the ini file using File->Open->INI.
This will load the configuration file and populate objects
in editing group.

You can choose if you want to flip UV (flips V) or if you want
to use model optimization.

Press compile to generate a new model file. In the newly
opened window type modelname.sam for animated models and
modelname.gsm for static ones.


## Download
[Download](https://github.com/ermaccer/Miracle3DDesigner/releases/latest/download/M3DDesigner.zip)


![Preview](https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/tools/m3d/example.png)