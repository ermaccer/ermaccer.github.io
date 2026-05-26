---
title: MKGExplorer
date: 2021-06-20 16:20:00 +0200
categories: [Tools, Archives]
tags: [dc, dreamcast, mkg, mk, geo, img]  
hidden: false
image: https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/tools/mkg/mkg_explorer.jpg
description: MKGExplorer allows you to convert files from Mortal Kombat Gold.
---

![Preview](https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/tools/mkg/mkgexplorer.png)

MKGExplorer allows you to convert files from and to Mortal Kombat Gold.


# Features
- Converts GEO models to OBJ or SMD
- Converts IMG files to BMP
- Saves any metadata required to rebuild both file types
- 3D model replacing support with an option to generate normals for problematic models


![Preview](https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/tools/mkg/preview.png)



<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/MKGExplorer/releases/latest/download/MKGExplorer.zip" role="button">
<i class="fas fa-download"></i>
Download
</a>


<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/MKGExplorer/" role="button">
<i class="fab fa-github"></i>
Source
</a>


# Building GEOs

## Getting GEO info
To build a new GEO file an original one needs to be dumped first. To get a rebuildable dump do:

1. In the menu bar, do `File->Open->Geometry (.GEO)`
2. Press `Export for Building` and pick a folder
3. As a reference, press `Export to OBJ` (with combine option ON) if your 3D software doesn't support batch import of files.

## GEO editing

The generated .ini file contains everything about the GEO file, amount of models, model data and so on. 

**Header Layout**

```ini
[Build.Settings]
Models = 33
Folder = RE_GEO_models
```

This section contains header information, `Folder` field can be edited to change to a different path if needed. 

**Model Layout**

Per each model there's a model section

```ini
[Model0]
Unk = 1
Models = 10

Model0 = model0\0.obj
Model0Unk = 0
Model0Unk2 = 0
Model1 = model0\1.obj
Model1Unk = 0
Model1Unk2 = 1
Model2 = model0\2.obj
# and so on
```

The ``Unk`` value is likely the texture ID from the associated .IMG file.

``Models`` value indicates how many submodels/strips are used. Per model ``Unk`` and ``Unk2`` values are unknown. They might be related to transparency or draw order.

``Model#NUMBER`` entry is the path to the .OBJ file that will be used. This is what can be directly edited with any 3D software. 
Because the geometry is stored as splits it might be hard to figure out which part is what. Use batch import on all .obj files or use the combined .obj file as a reference (Group named `G0` is `Model0` in the .ini file).

MKGExplorer will generate splits as needed, there's no need to replace all 10 parts manually in a model. The whole section can be replaced with:


```ini
[Model0]
Unk = 1
Models = 1

Model0 = Part0.obj
Model0Unk = 0
Model0Unk2 = 0
```

This will read `RE_GEO_models\Part0.obj` and generate any splits as needed during GEO creation.


<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://drive.google.com/file/d/1n_OvB48yeCFXLlbalDWwZvzX0AIaxee5/view?usp=drive_link" role="button">
<i class="fas fa-download"></i>
Download Example Model (Jax, JX_GEO)
</a>

<div class="alert bg-dark">
    This is the <a href="/posts/claude-mkg/">GTA3 Claude</a> model source.
</div>




## Creating GEO

Once its done, open the generated .ini file by using `File->Open INI`. This changes the program to work in build mode.

<div class="alert bg-dark">
By default, <b>Generate Normals</b> is active. It is recommended to keep this option ON, if automated normals aren't looking good in game it may be turned off to use normals from the OBJ file - be aware that normals amount must match the amount of vertices in that case!
</div>

`Create GEO` button will be available, press it and save the file. The output GEO is ready to be used in game

# Building IMGs

.IMG is the texture container for MKG. There can be multiple textures in a .IMG file.

To get a rebuildable dump do:

1. In the menu bar, do `File->Open->Image (.IMG)`
2. Press `Export to BMP` and pick a folder

This will save a .txt file (eg. JX_GEO.txt) with list of used BMP images. BMP images must be 16 bit XRGB images! This tool does not convert images.

If using GIMP, in advanced BMP saving options pick `X1 R5 G5 B5` to create a compatible file.

To build a .IMG, press `Build from TXT` in the `Image (.IMG)` area. Pick the .txt file then the destination and the tool will load any listed images from the same folder
as the .txt file.