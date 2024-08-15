---
title: Widescreen Fix
permalink: /posts/plugins/wsfix/agent-hugo
date: 2024-08-15 06:45:00 +0100
categories: [Modifications, Agent Hugo]
tags: [hugo, asi, pc, agent_hugo, widescreen]   
image: https://raw.githubusercontent.com/ermaccer/AgentHugo.WidescreenFix/master/hugo02.jpg
description: Modern resolution support.
hidden: false
---

Fixes 2D scaling and adjusts camera. Patches configuration tool to support all available resolutions.

<div class="alert bg-dark">
    This plugin was tested only with:
    <ul>
    <li>AgentHugo.exe - 3534848 bytes</li>
    <li>Config.exe - 2326528 bytes</li>
    </ul>
</div>


# Screenshots
<img class="img-fluid mx-auto" alt="1" src="https://raw.githubusercontent.com/ermaccer/AgentHugo.WidescreenFix/master/hugo01.jpg">
<img class="img-fluid mx-auto" alt="2" src="https://raw.githubusercontent.com/ermaccer/AgentHugo.WidescreenFix/master/hugo02.jpg">


# Download

<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/AgentHugo.WidescreenFix/releases/latest/download/AgentHugo.WidescreenFix.zip" role="button">
<i class="fas fa-download"></i>
Download
</a>
<br>
<a class="btn btn-block btn-dark bg-dark text-gray btn-lg" style="color: white;" href="https://github.com/ermaccer/AgentHugo.WidescreenFix/" role="button">
<i class="fab fa-github"></i>
Source
</a>


# Installation 

Extract **AgentHugo.WidescreenFix.zip** to root folder of Agent Hugo.

Archive breakdown:

 - d3d9.dll and ddraw.dll - [Ultimate ASI Loader](https://github.com/ThirteenAG/Ultimate-ASI-Loader/)
 - AgentHugo.WidescreenFix.asi
 - AgentHugo.ConfigPatch.asi
  
There's a copy of UAL because Config.exe imports ddraw while main executable doesn't.