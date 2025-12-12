---
layout: page
title: presentations
permalink: /presentations/
nav: true
nav_order: 4
---

## Invited Talks
{% bibliography_talks --file talks --query @talk[type=Invited Talk] %}

## Conference Talks
{% bibliography_talks --file talks --query @talk[type=Conference Talk] %}

## Posters
{% bibliography_talks --file talks --query @talk[type=Poster] %}

