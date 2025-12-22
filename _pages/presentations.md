---
layout: page
title: presentations
description: Presentations in reversed chronological order by categories, including presentations on conferences, project meetings, and competitions.
permalink: /presentations/
nav: true
nav_order: 4
---

<h2 class="key-subtitle">conference presentations</h2>
{% bibliography 
  --file talks
  --template bib-talk 
  --query @talk[type=Conference]
%}

<h2 class="key-subtitle">project report presentations</h2>
{% bibliography 
  --file talks
  --template bib-talk 
  --query @talk[type=Project] 
%}

<h2 class="key-subtitle">competition presentations</h2>
{% bibliography 
  --file talks 
  --template bib-talk 
  --query @talk[type=Competition] 
%}
