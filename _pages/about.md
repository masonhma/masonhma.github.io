---
layout: about
title: about
permalink: /
subtitle: |
  Graduate Research Assistant, Ph.D. Candidate<br>
  <a href="https://www.utidealab.com/" target="_blank">Manufacturing Intelligent Dynamics (MINDS) Lab</a><br>
  <a href="https://mtrc.utk.edu/" target="_blank">Machine Tool Research Center</a><br>
  <a href="https://www.utk.edu/" target="_blank">University of Tennessee</a>

profile:
  align: right
  image: portrait.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>Email: hma19@vols.utk.edu</p>
    <p>525 John D. Tickle Engineering Building, 817 Neyland Drive</p>
    <p>Knoxville, TN 37996-2315</p>

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

research_interests:
  - Solid-state additive manufacturing, machining, hybrid manufacturing, smart manufacturing
  - "Machine-tool-process-materials relation: mechanics, vibration, materials behaviors, CNC design"
  - Machine tool vibration theory and applications for machining and additive friction stir deposition
  - Analytical and numerical process modeling from machine tool to materials behaviors
  - Dynamical systems modeling, bifurcation, control and automation for manufacturing processes
  - Physics-based machine learning and artificial intelligence for modeling and optimization

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 3 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

I am a Ph.D. candidate at the Department of Industrial and Systems Engineering of The University of Tennessee, Knoxville, working with Drs. Tony Shi and Tony Schmitz. My research areas are manufacturing processes and systems innovations, with a focus on machining, metal additive manufacuting, hybrid, and smart manufacturing, to advance the next-generation design and manufacturing.


Before starting my Ph.D. journey, I received my BS degree in Automation Science and Engineering from Tsinghua University in 2014. I also received a MS degree in Management Science and Engineering from Peking University in 2017, and a MS degree in Industrial Engineering from The University of Wisconsin-Madison in 2019.


## education

<div class="education-list">
{% assign education = site.data.resume.education | sort: "startDate" | reverse %}
{% for edu in education %}
  <div class="row mb-4 align-items-center">
    <!-- Logo column -->
    <div class="col-3 col-md-2 d-flex justify-content-center align-items-center">
    {% if edu.logo %}
      <div class="edu-logo">
        <img
          src="{{ '/assets/img/education/' | append: edu.logo | relative_url }}"
          alt="{{ edu.institution }} logo"
          style="
                max-width: 70px;
                max-height: 70px;
                object-fit: contain;
              "
        >
      </div>
    {% endif %}
    </div>


    <!-- Text column -->
    <div class="col-9 col-md-10">
      <h4 class="mb-1">{{ edu.institution }}</h4>

      <p class="mb-1">
        {{ edu.studyType }}, {{ edu.area }},
        {{ edu.startDate | slice: 0,4 }}–{{ edu.endDate | slice: 0,4 }}
      </p>

      {% if edu.extra %}
        {% for line in edu.extra %}
          <p class="mb-0">{{ line }}</p>
        {% endfor %}
      {% endif %}
    </div>

  </div>
{% endfor %}
</div>




## research interests

<ul>
{% for item in page.research_interests %}
  <li>{{ item }}</li>
{% endfor %}
</ul>
