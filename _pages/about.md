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

<div class="container" style="max-width: 900px; margin-top: 2rem;">
  {% assign educations = site.data.resume.education | sort: 'startDate' | reverse %}
  {% for edu in educations %}
    <div class="row mb-4 align-items-center edu-row">
      <!-- Logo column -->
      <div class="col-3 col-md-2 d-flex justify-content-center">
        {% if edu.logo %}
          <div class="edu-logo-wrap">
            <img
              src="{{ '/assets/img/education/' | append: edu.logo | relative_url }}"
              alt="{{ edu.institution }} logo"
              class="edu-logo"
            >
          </div>
        {% endif %}
      </div>

      <!-- Text column -->
      <div class="col-9 col-md-10">
        <div class="edu-text">
          <h4 class="mb-1 edu-title">{{ edu.institution }}</h4>
          <div class="edu-subtitle">
            {{ edu.studyType }}, {{ edu.area }}, {{ edu.startDate }}–{{ edu.endDate }}
          </div>

          {% if edu.extra %}
            <ul class="mb-0 mt-1">
              {% for line in edu.extra %}
                <li>{{ line }}</li>
              {% endfor %}
            </ul>
          {% endif %}
        </div>
      </div>
    </div>
  {% endfor %}
</div>

<style>
  /* Fixed logo box + true centering */
  .edu-logo-wrap{
    width: 90px;           /* change once: 80/90/100 */
    height: 90px;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .edu-logo{
    max-width: 100%;
    max-height: 100%;
    object-fit: contain;   /* crucial */
    display: block;
  }

  /* Make text start at the same x-position and look consistent */
  .edu-text{ padding-left: 6px; }
  .edu-title{ line-height: 1.1; }
  .edu-subtitle{ font-size: 1.05rem; }
</style>




## Research Interests

<ul>
{% for item in page.research_interests %}
  <li>{{ item }}</li>
{% endfor %}
</ul>
