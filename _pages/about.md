---
layout: about
title: about
permalink: /
subtitle: |
  Ph.D. Candidate - Industrial Engineering<br>
  <a href="https://utorii.com/gate-awards/" target="_blank">GATE Fellow 2021, 2022</a> | <a href="https://hammer.osu.edu/about-us/councils-and-board" target="_blank">NSF ERC-HAMMER SLC Convergence Research Lead, 2024</a><br>
  <a href="https://www.utidealab.com/" target="_blank">Manufacturing Intelligent Dynamics (MINDS) Lab</a><br>
  <a href="https://mtrc.utk.edu/" target="_blank">Machine Tool Research Center</a><br>
  <a href="https://www.utk.edu/" target="_blank">University of Tennessee, Knoxville</a>

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

awards:
  - NSF HAMMER ERC Perfect Pitch Competition Winner (UTK site), 2024
  - Graduate Student Senate Travel Award, University of Tennessee, Knoxville, 2023
  - Graduate Advancement Training and Education (GATE) Fellowship, Science Alliance, University of Tennessee, Knoxville, 2021, 2022
  - Lloyd W Crawford Fellowship, University of Tennessee, Knoxville, 2020, 2021.

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 3 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

I am a Ph.D. candidate at the Department of Industrial and Systems Engineering of The University of Tennessee, Knoxville, working with Drs. <a href="https://www.utidealab.com/director-biography" target="_blank">Tony Shi</a> and <a href="https://mtrc.utk.edu/tony-schmitz/" target="_blank">Tony Schmitz</a>. My research areas are manufacturing processes and systems innovations, with a focus on machining, additive friction stir deposition (AFSD), wire-arc additive manufacturing (WAAM), hybrid and smart manufacturing, to advance the next-generation design and manufacturing. Before starting my Ph.D. journey, I received my BS degree in Automation Science and Engineering from Tsinghua University in 2014. I also received a MS degree in Management Science and Engineering from Peking University in 2017, and a MS degree in Industrial Engineering from The University of Wisconsin-Madison in 2019.

As a Graduate Research Assistant, my resarch has been supported by <a href="https://hammer.osu.edu/" target="_blank">NSF Engineering Research Center for Hybrid Autonomous Manufacturing Moving from Evolution to Revolution (ERC-HAMMER)</a>, <a href="https://seamtn.utk.edu/" target="_blank">DoD Southeastern Advanced Machine Tools Network (SEAMTN)</a>, <a href="https://research.utk.edu/aitn/" target="_blank">AI Tennessee Initiative</a>, and <a href="https://utorii.com/gate-awards/" target="_blank">The University of Tennessee-Oak Ridge Innovation Institute (UT-ORII)</a>.




## education

<div class="row">
  <!-- LEFT CONTENT COLUMN (same width as text above) -->
  <div class="col-12 col-md-8">

    <div class="education-list">
    {% assign education = site.data.resume.education | sort: "startDate" | reverse %}
    {% for edu in education %}
      <div class="row mb-4 align-items-center">

        <!-- Logo column -->
        <div class="col-3 col-md-2 d-flex justify-content-center align-items-center">
          {% if edu.logo %}
            <img
              src="{{ '/assets/img/education/' | append: edu.logo | relative_url }}"
              alt="{{ edu.institution }} logo"
              style="max-width: 60px; max-height: 60px; object-fit: contain;"
            >
          {% endif %}
        </div>

        <!-- Text column -->
        <div class="col-9 col-md-10">
          <h4 class="mb-1" style="font-size: 1.2rem;">
            {% if edu.url %}
              <a href="{{ edu.url }}" target="_blank" rel="noopener">
                {{ edu.institution }}
              </a>
            {% else %}
              {{ edu.institution }}
            {% endif %}
          </h4>

          <!-- Study type (row 1) -->
          <div class="education-degree">
            {{ edu.studyType }}, {{ edu.area }}
          </div>
    
          <!-- Dates (row 2) -->
          <div class="education-dates">
            {{ edu.startDate | slice: 0,4 }}–{{ edu.endDate | slice: 0,4 }}
          </div>
        </div>

      </div>
    {% endfor %}
    </div>

  </div>
</div>





## research interests
<ul>
{% for item in page.research_interests %}
  <li>{{ item }}</li>
{% endfor %}
</ul>



## awards and recognitions
<ul>
{% for item in page.awards %}
  <li>{{ item }}</li>
{% endfor %}
</ul>
