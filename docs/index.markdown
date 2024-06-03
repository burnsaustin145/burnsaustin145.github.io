---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
# Projects

## AI

### Undergraduate Research - Fine-tuning
|Fine-tuning|LLM|
(in progress)
A project using fine-tuning to investigate and improve the truthfulness of chat gpt-turbo 3.5

### LLM for the Contemporary History of Iran
|RAG|LLM|
(in progress)
This project integrates current political and
historical data into an interactive AI model, greatly improving access to information on Iran’s contemporary history.

## Cyberphysical Systems

### Carla PID Controller
|PID|Carla|Autonomous Driving|
[See project on GitHub](https://github.com/burnsaustin145/carla_PID){:target="_blank"}

Created a proportional-integral-derivative controller for car throttle and brake control. Using object detection sensors alone I was able to create a system which navigates in heavy traffic without collisions. 

<p align="center">
  <img src="/assets/states1.png" alt="CF makeup" width="100%"/>
  <em>A state transition diagram of the system.</em>
</p>


<p align="center">
  <img src="/assets/clamp1.png" alt="CF makeup" width="100%"/>
  <em>We see the final result of speed over time, with minimal overshoot or oscillation.</em>
</p>


## Statistical Analysis

### NBA CrowdFactor Statistic
|Logistic Regression|Data Wrangling|  
[See project on GitHub](https://github.com/burnsaustin145/Statistical-Analysis-NBA){:target="_blank"}

Developed a novel statistic to represent team confidence. This work was done to fulfill a final project requirement for a gradute-level statistics course.

<p align="center">
  <img src="/assets/crowdFactor_blocks_stls_tran.png" alt="CF makeup" width="100%"/>
</p>

CrowdFactor statistic is created by applying a logit function to the stadium fill percentage, and then reflected about 0.5 for away teams.

<p align="center">
  <img src="/assets/cf_only_tran.png" alt="CF results" width="100%"/>
</p>

CrowdFactor was shown to predict the result of a game better than random. 


### Detroit Crime Heatmap
|Graphical Statistics|  
[See project on GitHub](https://github.com/burnsaustin145/Heat-Map){:target="_blank"}  

Created this heatmap in R to visualize crime in Detroit over the last 100 years. 

<p align="center">
  <img src="/assets/crime_heatmap_03_tran1.png" alt="heatmap" width="100%"/>
</p>

*Heatmap uses [Stamen Map](https://rdrr.io/cran/ggmap/man/get_stamenmap.html){:target="_blank"} and [this open data](https://data.detroitmi.gov/datasets/detroitmi::rms-crime-incidents/explore?location=42.357655%2C-83.048440%2C15.00&showTable=true){:target="_blank"}.*


## Semantic Networks
My interest in AI began with the concept of semantic networks, an idea I learned from Douglas Hofstadter's [GEB](https://en.wikipedia.org/wiki/G%C3%B6del,_Escher,_Bach){:target="_blank"}. Since then I have been interested in representing and manipulating knowledge in graph/hypergraph based structures. 

Below is one such abstract structure.
<p align="center">
  <img src="/assets/complex_object_tran.png" alt="complex object" width="100%"/>
</p>
