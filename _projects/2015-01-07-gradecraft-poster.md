---
layout: default
previous_url: dashboards
next_url: gradecraft-site-redesign
title: gradecraft-poster
name: GradeCraft Poster
---
{% assign page_data = site.data[page.slug] %}

<section class="project-page">
  <div class="section-header"><h1>{{page_data.name}}</h1>
    <ul class="project-roles">
      {% for item in page_data.role %}
        <li>{{ item }}</li>
      {% endfor %}
    </ul>
  </div>

  <div class="project-data">
    <div class="case-study challenge">
      <h2>Overview</h2>
      <p>{{page_data.overview}}</p>
    </div>
    <div class="project-photo">
      <img src="/img/{{page_data.project_image_1}}">
    </div>
  </div>

</section>