---
layout: page
title: presentations
permalink: /presentations/
nav: true
nav_order: 4
---

<h2 class="presentations-section">conference presentations</h2>
{% bibliography 
  --file talks
  --template bib-talk 
  --query @talk[type=Conference]
%}

<h2 class="presentations-section">conference presentations</h2>
{% bibliography 
  --file talks
  --template bib-talk 
  --query @talk[type=Project] 
%}

<h2 class="presentations-section">conference presentations</h2>
{% bibliography 
  --file talks 
  --template bib-talk 
  --query @talk[type=Competition] 
%}
