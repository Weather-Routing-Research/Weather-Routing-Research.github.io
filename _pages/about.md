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
  /* Add CSS styles to adjust the layout */
  .latest-news-container {
    display: flex;
    justify-content: space-between; /* Space evenly between items */
  }

  .news-item {
    text-align: center;
    max-width: 30%; /* Adjust the maximum width as needed */
    position: relative; /* Create a relative positioning context */
    overflow: hidden; /* Hide overflowing content */
  }

  .news-item img {
    width: 100%; /* Set width to 100% to fill the container */
    height: 0; /* Set initial height to 0 */
    padding-bottom: 75%; /* Create a 4:3 aspect ratio (3/4 * 100) */
    object-fit: cover; /* Crop the image to fit the container */
  }

  /* Center the title */
  .news-item h3 {
    position: absolute;
    top: 50%; /* Center vertically */
    left: 50%; /* Center horizontally */
    transform: translate(-50%, -50%);
    background-color: rgba(255, 255, 255, 0.8); /* Add a semi-transparent background for readability */
    padding: 10px;
  }
</style>
