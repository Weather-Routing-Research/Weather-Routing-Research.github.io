---

title: "Connected Graph Partitioning with Aggregated and Non-aggregated Gap Objective Functions"
collection: publications
permalink: /publication/2023/graph-partitioning
excerpt: "This research introduces the notion of aggregated gap in graph partitioning, expanding on the traditional gap objectives."
date: 2023-08-10
venue: "Networks"
paperurl: "https://doi.org/10.1002/net.22181"
featured_image: "https://onlinelibrary.wiley.com/cms/asset/a736d24f-d9f6-48c1-9a12-ae0cf8540526/net22181-fig-0003-m.jpg"

---

### Abstract

Partitioning graphs into connected components presents unique challenges, especially when vertex weight balancing becomes pivotal. Traditional objective functions have usually considered the gap or range of the partition's components, defined as the weight difference between the maximum and minimum vertices within a component. This study introduces a nuanced approach: the aggregated gap, representing the cumulative differences between vertex weights and the component's minimum vertex weight. 

This new perspective brings forth connected partitioning problems, the primary focus of which is the components' aggregated gap. NP-hardness results, acquired for these problems on general graphs, underline their computational complexity. The team has proposed mathematical programming formulations using flow-based constraints, ensuring connectivity within partitions. Interestingly, these new formulations, though crafted for the aggregated gap, also apply seamlessly to classical non-aggregated gap problems.

Extensive computational experiments have been the cornerstone of this research. Tests were conducted on squared grids and randomly generated graphs with up to 120 vertices. Components in these experiments ranged between 2 to 9. The research doesn't just stop at presenting these results; it delves deep into comparing multiple formulations, shedding light on their relative efficiencies.

[**Download the full paper here**]({{ page.paperurl }})

---

### Authors & Affiliations

- **Elena Fernández**  
  _Department of Statistics and Operations Research_  
  University of Cádiz  
  Spain

- **Isabella Lari**  

- **Justo Puerto**  

- **Federica Ricca**  

- **Andrea Scozzari**
