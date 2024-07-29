---
title: "WeatherRouting Bench 1.0 Now Live!"
date: 2024-07-29
permalink: /news/2024/benchmark-website
excerpt: "We have released the first benchmark for weather routing. Towards comparative research in maritime optimization!"
featured_image: "https://weathernavigation.com/images/2024-07-29-benchmark-website.png"
tags:
  - weather routing
  - optimization
  - naval engineering
  - website
  - benchmark
---

The Weather Navigation project is excited to announce the release of [WeatherRouting Bench 1.0](https://benchmark.weathernavigation.com/), the first comprehensive benchmark for weather routing. This tool addresses a significant gap in weather routing research: the absence of a standardized method for comparing algorithms.

Our benchmark provides a website with Python code to help researchers utilize weather data, test routes, and apply a consistent cost function for evaluating different methods. We also present optimization problems based on real shipping routes, each including a standard route as a baseline for comparison.

In the forthcoming paper accompanying this benchmark release, we explore how different problem settings impact optimization. We analy how the average cost of a journey varies with sailing speeds, ocean regions, and times of the year. By offering this benchmark, we aim to simplify the comparison of research efforts in weather routing.

<a href="https://benchmark.weathernavigation.com/" class="button">Explore WeatherRouting Bench 1.0</a>

As a first entry to the benchmark, our next paper introduces A⋆-FMS: an algorithm that combines A⋆ graph search with a discrete Newton-Jacobi method. This hybrid approach leverages the global search capabilities of graph methods and the local optimization strength of gradient descent methods. With optimal configuration, A⋆-FMS reduces travel time by 1.4% when sailing at 12 knots and 3.6% at 6 knots, compared to the orthodromic route.

Stay tuned for the release of our next paper!

This research is supported by:

- [BBVA Foundation](https://www.fbbva.es/) via the project "Mathematical optimization for a more efficient, safer and decarbonized maritime transport".

- Spanish [Agencia Estatal de Investigación](https://www.aei.gob.es/) under grant  TED2021-129455B-I00, "Optimization of maritime routes with real time oceanographic and meteorological data".
