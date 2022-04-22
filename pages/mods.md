---
layout: page
title: Mods
---
<style>
.mod {
 transition: transform 0.4s;
 padding-bottom: 2em;
}
.mod:hover{
 transform: scale(1.10);
}
</style>
<!-- todo -->
<div class="row">
  <div id="post-wrapper" class="col-12 col-lg-11 col-xl-12">
  <h1 class="text-center">Mods</h1>
  <hr>

  {% assign mods= "manhunt,manhunt-2,injustice-gods-among-us,injustice-2,mortal-kombat-ii,mortal-kombat-deception,mortal-kombat-unchained,mortal-kombat-armageddon,mortal-kombat-komplete-edition,mortal-kombat-x,mortal-kombat-11,ultimate-marvel-vs-capcom-3,the-punisher,scarface,battle-mages-sign-of-darkness,sniper-elite-nazi-zombie-army" | split: ',' %}

  {% for mod in mods %}
        <div class="text-center w-25 col-sm-4 float-left">
          <a href="{{ site.baseurl }}/categories/{{ mod }}/" >
             <img class="img-fluid mod" src="../../assets/mods/{{ mod }}.jpg" alt="{{ mod }}">
          </a>
        </div>
  {% endfor %}    

  </div>
</div> <!-- .row -->

  <hr>
  <div class="text-center">
    <a class="btn btn-dark bg-dark text-gray btn-lg" style="color: white;" href="{{ site.baseurl }}/categories/widescreen-fixes/" role="button">
     Widescreen Fixes
    </a>
  </div>
