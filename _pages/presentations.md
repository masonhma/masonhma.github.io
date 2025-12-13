---
layout: page
title: presentations
permalink: /presentations/
nav: true
nav_order: 4
---

<h2 style="text-align:center; color:#d63384;">Conference presentations</h2>
{% bibliography --file talks --query @talk[type=Conference Talk] %}

<h2 style="text-align:center; color:#d63384;">Posters</h2>
{% bibliography --file talks --query @talk[type=Poster] %}

