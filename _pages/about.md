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

<!-- Add this section to display the five latest papers in bulletpoints -->
<h2>Latest Papers</h2>
<ul class="latest-articles-container">
  {% for paper in site.publications limit:5 %}
    <li><a href="{{ paper.url }}">{{ paper.title }}</a></li>
  {% endfor %}
</ul>

<!-- Add this section to display the five latest talks in bulletpoints -->
<h2>Latest Talks</h2>
<ul class="latest-talks-container">
  {% for talk in site.talks limit:5 %}
    <li><a href="{{ talk.url }}">{{ talk.title }}</a></li>
  {% endfor %}
</ul>

<!-- Add this section to display the three latest news articles horizontally -->
<h2>Latest News</h2>
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

<style>
  /* Adjusts the layout of the news container */
  .latest-news-container {
    display: flex;
    justify-content: space-between; /* Space evenly between items */
  }

  /* Style specifications for each news item */
  .news-item {
    text-align: center;
    max-width: 30%; /* Adjust the maximum width as needed */
    position: relative; /* Create a relative positioning context */
    overflow: hidden; /* Ensure nothing spills out of the box */
  }

  /* Styles for the image of the news item */
  .news-item img {
    width: 100%;
    display: block; /* Removes any gaps below the image */
    object-fit: cover; /* Crop the image to fit the container */
    border-radius: 10px; /* Add rounded borders */
    transition: transform 0.3s; /* Smooth zoom on hover for a more interactive effect */
  }

  /* Add a zoom effect when hovering over the news item */
  .news-item:hover img {
    transform: scale(1.05); /* Slight zoom effect on hover */
  }

  /* Center the title over the image */
  .news-item h3 {
    position: absolute;
    bottom: 0; /* Position the title at the bottom of the image */
    width: 100%; /* Use the full width of the parent */
    background-color: rgba(0, 0, 255, 0.6); /* Blue background with 60% opacity for readability */
    color: white; /* Text color set to white for visibility against the blue */
    padding: 10px 0; /* Padding at top and bottom */
    margin: 0; /* Remove any default margins */
    border-radius: 0 0 10px 10px; /* Rounded borders only at the bottom of the title */
    text-align: center; /* Center align the text */
  }
</style>
