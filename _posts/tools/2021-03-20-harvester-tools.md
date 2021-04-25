---
title: Harvester Tools
date: 2021-03-20 14:39:00 +0200
categories: [Tools, General]
tags: [harvester, archive, bm, bmp,text]  
pin: true
---


# HArchive

Extracts archive files such as HARVEST.DAT and SOUND.DAT

### Usage
Simply drag an archive onto the executable.

[Download](https://github.com/ermaccer/HArchive/releases/)


# HImage
Converts .BM images to viewable BMP - you'll need to
find proper .PAL file for the images.

Most HEADS/INVENTORY images use INVHELP.PAL file.

### Usage

```himage -e -p PALFILE.PAL IMAGE.BM```


![Preview](https://raw.githubusercontent.com/ermaccer/ermaccer.github.io/gh-pages/assets/tools/harvest/himage_preview.png)

[Download](https://github.com/ermaccer/HImage/releases)




# HScramble
Makes Harvester text files readable.
Tested with .SCR and .IDX text files.

### Usage
Simply drag any Harvester text file onto the executable.

### Before
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

### After

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
[Download](https://github.com/ermaccer/HScramble/releases)
