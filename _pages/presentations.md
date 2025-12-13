---
layout: page
title: presentations
permalink: /presentations/
nav: true
nav_order: 4
---

<h2 style="text-align:center; color:#d63384;">conference presentations</h2>
{% bibliography 
  --file talks
  --template bib-talk 
  --query @talk[type=Conference]
%}

<h2 style="text-align:center; color:#d63384;">project report presentations</h2>
{% bibliography 
  --file talks
  --template bib-talk 
  --query @talk[type=Project] 
%}

<h2 style="text-align:center; color:#d63384;">competition presentations</h2>
{% bibliography 
  --file talks 
  --template bib-talk 
  --query @talk[type=Competition] 
%}
