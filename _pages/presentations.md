---
layout: page
title: presentations
permalink: /presentations/
nav: true
nav_order: 4
---

<div class="presentations">

{% bibliography_talks %}

</div>


<h2 style="text-align:center; color:#d63384;">Conference presentations</h2>
{% bibliography 
  --file talks
  --template bib 
  --query @talk[type=Conference]
%}

<h2 style="text-align:center; color:#d63384;">Project report</h2>
{% bibliography 
  --file talks
  --template bib 
  --query @talk[type=Project] 
%}

<h2 style="text-align:center; color:#d63384;">Competition presentations</h2>
{% bibliography 
  --file talks 
  --template bib 
  --query @talk[type=Competition] 
%}
