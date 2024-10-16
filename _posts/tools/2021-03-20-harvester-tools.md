---
title: Harvester Tools
date: 2021-03-20 14:39:00 +0200
categories: [Tools, General]
tags: [harvester, archive, bm, bmp,text]  
hidden: false
image: https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/tools/harvest/harvester_tools.jpg
description: A collection of tools for the DOS game - Harvester.
---


# HArchive
Extracts archive files such as HARVEST.DAT and SOUND.DAT

## Usage
Simply drag an archive onto the executable.

<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/HArchive/releases/" role="button">
<i class="fas fa-download"></i>
Download
</a>

# HImage
Converts .BM images to viewable BMP - you'll need to
find proper .PAL file for the images.

Most HEADS/INVENTORY images use INVHELP.PAL file.

## Usage

```himage -e -p PALFILE.PAL IMAGE.BM```

<img class="img-fluid mx-auto" alt="menu" src="{% link assets/tools/harvest/himage_preview.png %}">

<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/himage/releases/" role="button">
<i class="fas fa-download"></i>
Download
</a>


# HAImage
Converts .ABM images to viewable BMP frames - you'll need to
find proper .PAL file for the images.

Most character images use INVHELP.PAL file.

## Usage

```haimage -e -p PALFILE.PAL IMAGE.ABM```

<img class="img-fluid mx-auto" alt="menu" src="{% link assets/tools/harvest/abm_preview.png %}">

<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/haimage/releases/" role="button">
<i class="fas fa-download"></i>
Download
</a>



# HScramble
Makes Harvester text files readable.
Tested with .SCR and .IDX text files.

## Usage
Simply drag any Harvester text file onto the executable.

## Before
```
›
ŔßÄÁŠĂÄĂŢ
ť
óĎŮ•
››
ăŠÄĎĎÎŠŮĹÇĎŠÂĎĆÚ„„„ŠçĂŮŢĎŘ„„„•
›ź
úĹŮŢÇËŮŢĎŘŠčĹÓĆĎ„ŠŠýÂËŢŠÉËÄŠăŠÎĹŠÓĹßŠĚĹŘŠŢĹÎËÓ•
```

## After

```
1
"junk init"
7
"Yes?"
11
"I need some help... Mister...?"
15
"Postmaster Boyle.  What can I do you for today?"
25
"Sorry, youngster, we're out of applications right now."
```
<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/HScramble/releases" role="button">
<i class="fas fa-download"></i>
Download
</a>
