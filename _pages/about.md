---
permalink: /
title: "Optimization of maritime routes for a more efficient, safer and decarbonized transport"
excerpt: "Optimization of maritime routes for a more efficient, safer and decarbonized transport"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<p align="center"><img src="https://weathernavigation.com/images/banner.png" alt="Banner" width="100%"/></p>

[IE University](https://www.ie.edu/) and [Universidad de Cádiz](https://www.uca.es/) promote this interdisciplinary project aimed at providing algorithms to calculate safe and optimized shipping routes for reduced fuel consumption and emissions, taking into account real time oceanographic and meteorological information. The necessary data will be collected from public repositories such as NOAA, Copernicus or HYCOM, and they include predictions for ocean currents, wind and waves. Detailed models will be built to estimate the fuel consumption and emissions of every vessel as a function of its characteristics (displacement, hull length, engine power), cruising speed and sea conditions (currents, waves and wind).

This task involves both reviewing the vast literature on this subject and possibly fitting our own data driven models in case routes and consumption data become available. Next, optimization algorithms will be developed to find optimal routes and calculate fuel savings and estimated time of arrival (ETA) at the port destination. Profiting from better sea and weather conditions has been shown to save on average 3-7% of fuel. This is a challenging project whose success depends on the cross fertilization and cooperation between oceanographers, naval engineers, data scientists, mathematicians and software developers.

The goal is both to improve the state of the art algorithms for weather routing, publishing our results in specialized scientific journals and to develop software tools that address this important industrial problem for shipping companies.

<!-- Style -->
{% include head.html %}

<!-- Add this section to display the latest papers in bulletpoints -->
<!--
<h2>Latest Papers</h2>
<ul class="latest-articles-container">
  {% assign sorted_papers = site.publications | sort: 'date' | reverse %}
  {% for paper in sorted_papers limit:3 %}
    <li><a href="{{ paper.url }}">{{ paper.title }}</a></li>
  {% endfor %}
</ul>
-->

<!-- Add this section to display the chosen papers in bulletpoints -->
{% assign trending_papers = "/publications/2023/comparative/,/publications/2023/hybrid-search/,/publications/2023/emissions/" | split: "," %}

<h2>Latest Papers</h2>
<ul class="latest-articles-container">
  {% for permalink in trending_papers %}
    {% assign paper = site.publications | where: "permalink", permalink | first %}
    <li><a href="{{ paper.url }}">{{ paper.title }}</a></li>
  {% endfor %}
</ul>

<a href="https://weathernavigation.com/publications/" class="button">See All Publications</a>

<!-- Add this section to display the latest talks in bulletpoints -->
<h2>Latest Talks</h2>
<ul class="latest-talks-container">
  {% assign sorted_talks = site.talks | sort: 'date' | reverse %}
  {% for talk in sorted_talks limit:3 %}
    <li><a href="{{ talk.url }}">{{ talk.title }}</a></li>
  {% endfor %}
</ul>

<a href="https://weathernavigation.com/talks/" class="button">See All Talks</a>

<!-- Add this section to display the three latest news articles horizontally -->
<!-- <h2>Latest News</h2>
<div class="latest-news-container">
  {% for post in site.posts limit:3 %}
    <div class="news-item">
      <a href="{{ post.url }}">
        <img src="{{ post.featured_image }}" alt="{{ post.title }}" style="max-width: 100%; height: auto;">
        <h3>{{ post.title }}</h3>
      </a>
    </div>
  {% endfor %}
</div>
-->

<!-- Add this section to display three chosen news articles horizontally -->
{% assign trending_posts = "/news/2023/european-parliament/,/news/2023/wimobo/,/news/2023/halifax/" | split: "," %}

<h2>Trending News</h2>
<div class="latest-news-container">
  {% for permalink in trending_posts %}
    {% assign post = site.posts | where: "permalink", permalink | first %}
    <div class="news-item" style="position: relative;">
      <a href="{{ post.url }}">
        <img src="{{ post.featured_image }}" alt="{{ post.title }}" style="max-width: 100%; height: auto;">
        <h3>
          {% if post.abbreviated_title %}
            {{ post.abbreviated_title }}
          {% else %}
            {{ post.title }}
          {% endif %}
        </h3>
      </a>
    </div>
  {% endfor %}
</div>

<a href="https://weathernavigation.com/news/" class="button">See All News</a>

---

<a href="https://demo.weathernavigation.com/" class="button">Demo</a>

---

This research is supported by:

- [BBVA Foundation](https://www.fbbva.es/) via the project "Mathematical optimization for a more efficient, safer and decarbonized maritime transport".

- Spanish [Agencia Estatal de Investigación](https://www.aei.gob.es/) under grant  TED2021-129455B-I00, "Optimization of maritime routes with real time oceanographic and meteorological data".

<div style="display: flex; justify-content: center;">
  <div style="flex: 35%; margin-right: 10px;">
    <img src="https://weathernavigation.com/images/banner-bbva.png" alt="Banner BBVA" style="width: 100%; height: auto;"/>
  </div>
  <div style="flex: 65%; margin-left: 10px;">
    <img src="https://weathernavigation.com/images/banner-aei.png" alt="Banner AEI" style="width: 100%; height: auto;"/>
  </div>
</div>
