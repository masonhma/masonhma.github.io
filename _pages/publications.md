---
layout: page
permalink: /publications/
title: publications
description: Publications in reversed chronological order by categories, including refereed journal papers, under review, working papers, and refereed conference proceedings.
nav: true
nav_order: 3
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}


<h2 class = "key-subtitle">refereed journal papers</h2>
{% bibliography 
  --file papers
  --template bib 
  --query @article[group=Journal]
%}


<h2 class = "key-subtitle">under review</h2>
{% bibliography 
  --file papers
  --template bib 
  --query @article[group=Review]
%}


<h2 class = "key-subtitle">working papers</h2>
{% bibliography 
  --file papers
  --template bib 
  --query @article[group=Working]
%}


<h2 class = "key-subtitle">refereed conference proceedings</h2>
{% bibliography 
  --file papers
  --template bib 
  --query @inproceedings
%}
