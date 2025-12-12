---
layout: about
title: about
permalink: /
subtitle: <a href='https://www.utidealab.com/'>MINDS Lab</a>, <a href='https://www.utk.edu/'>University of Tennessee, Knoxville</a>

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
  - Machine-tool-process-materials relation: mechanics, vibration, materials behaviors, CNC design
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


Write your biography here. Tell the world about yourself. Link to your favorite [subreddit](http://reddit.com). You can put a picture in, too. The code is already in, just name your picture `prof_pic.jpg` and put it in the `img/` folder.

Put your address / P.O. box / other info right below your picture. You can also disable any of these elements by editing `profile` property of the YAML header of your `_pages/about.md`. Edit `_bibliography/papers.bib` and Jekyll will render your [publications page](/al-folio/publications/) automatically.

Link to your social media connections, too. This theme is set up to use [Font Awesome icons](https://fontawesome.com/) and [Academicons](https://jpswalsh.github.io/academicons/), like the ones below. Add your Facebook, Twitter, LinkedIn, Google Scholar, or just disable all of them.

## Education

<div class="education-list">
{% assign education = site.data.resume.education | sort: "startDate" | reverse %}
{% for edu in education %}
  <div class="row mb-4 align-items-center">

    <!-- Logo column -->
    <div class="col-3 col-md-2 text-center">
      {% if edu.logo %}
        <img
          src="{{ '/assets/img/education/' | append: edu.logo | relative_url }}"
          alt="{{ edu.institution }} logo"
          style="max-width: 90px;"
        >
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



## Research Interests

<ul>
{% for item in page.research_interests %}
  <li>{{ item }}</li>
{% endfor %}
</ul>
