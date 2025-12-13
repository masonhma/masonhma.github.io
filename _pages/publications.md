---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order.
nav: true
nav_order: 3
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}


<h2 style="text-align:center; color:#d63384;">Refereed journal papers</h2>
{% bibliography 
  --file papers
  --template bib 
  --query @talk[type=Journal]
%}


<h2 style="text-align:center; color:#d63384;">Under review</h2>
{% bibliography 
  --file papers
  --template bib 
  --query @talk[type=Review]
%}


<h2 style="text-align:center; color:#d63384;">Working papers</h2>
{% bibliography 
  --file papers
  --template bib 
  --query @talk[type=Working]
%}


<h2 style="text-align:center; color:#d63384;">Refereed conference proceedings</h2>
{% bibliography 
  --file papers
  --template bib 
  --query @talk[type=Conference]
%}
