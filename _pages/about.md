---
permalink: /
title: "Mathematical optimization for a more efficient, safer and decarbonized maritime transport"
excerpt: "Mathematical optimization for a more efficient, safer and decarbonized maritime transport"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

[BBVA Foundation](https://www.fbbva.es/) and [IE University](https://www.ie.edu/) promote this interdisciplinary project aimed at providing algorithms to calculate safe and optimized shipping routes for reduced fuel consumption and emissions, taking into account real time oceanographic and meteorological information. The necessary data will be collected from public repositories such as NOAA, Copernicus or HYCOM, and they include predictions for ocean currents, wind and waves. Detailed models will be built to estimate the fuel consumption and emissions of every vessel as a function of its characteristics (displacement, hull length, engine power), cruising speed and sea conditions (currents, waves and wind).

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
{% assign trending_posts = "/posts/2023/06/08/european-parliament/,/posts/2023/07/10/wimobo/,/posts/2023/08/15/halifax-research/" | split: "," %}

<h2>Latest Papers</h2>
<ul class="latest-articles-container">
  {% assign sorted_papers = site.publications | sort: 'date' | reverse %}
  {% for paper in sorted_papers limit:3 %}
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
{% assign trending_posts = "/posts/2023/european-parliament/,/posts/2023/wimobo/,/posts/2023/halifax/" | split: "," %}

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
