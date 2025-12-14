---
layout: page
title: Experiences
permalink: /experiences/
nav: true
nav_order: 3
---

{% assign data = site.data.experiences %}

<h2>Professional Experience</h2>
{% include experiences/professional_experiences.liquid data=data.professional_experiences %}

<h2>Teaching Experience</h2>
{% include experiences/teaching_experiences.liquid data=data.teaching_experiences %}

<h2>Reviewing Activities</h2>
{% include experiences/reviewers.liquid data=data.reviewers %}

<h2>Professional Services</h2>
{% include experiences/services.liquid data=data.services %}

<h2>Skills</h2>
{% include experiences/skills.liquid data=data.skills %}

<h2>Professional Membership</h2>
{% include experiences/membership.liquid data=data.membership %}

