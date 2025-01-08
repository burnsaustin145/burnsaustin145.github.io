---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
# Projects

## AI

### Undergraduate Research - Fine-tuning
|Fine-tuning|LLM|  
[See project on GitHub](https://github.com/burnsaustin145/FineTuning){:target="_blank"}  
A project using fine-tuning to investigate and improve the truthfulness of chat gpt-turbo 3.5
- Hundreds of fine-tuning examples were created and utilized with the OpenAI api, and tested with TruthfulQA data 
- Insufficencies in current research were identified along with future areas of inquiry

### LLM for the Contemporary History of Iran
|RAG|LLM|JavaScript|Firebase|  
This project integrates current political and
historical data into an interactive AI model, greatly improving access to information on Iran’s contemporary history.
 - [Persian Mind](https://huggingface.co/universitytehran/PersianMind-v1.0){:target="_blank"}, a Llama3 model was used in conjunction with retrieval augmented generation on academic resources
 - I designed this system and deployed it as a web application along with a quantized version of the LLM on our personal server with limited resources 
 - Not seen on github due to ownership conflicts

## Statistical Analysis

### NBA CrowdFactor Statistic
|Logistic Regression|Data Wrangling|  
[See project on GitHub](https://github.com/burnsaustin145/Statistical-Analysis-NBA){:target="_blank"}

A novel statistic was developed to represent team confidence. This work was done to fulfill a final project requirement for a graduate-level statistics course. 

The crowdfactor is defined as the percentage of stadium capacity passed through a sigmoid function, effectively amplifying the effect of a very full stadium on the home or away team -- the effect is inverted for the away team. Below we see a vague relationship between the crowdfactor and blocks, steals, and points.

<p align="center">
  <img src="/assets/crowdFactor_blocks_stls_tran.png" alt="CF makeup" width="100%"/>
</p>

A team confidence statistic was then created using a combination of crowdfactor, blocks, and steals which was shown to predict the result of a game better than random -- as seen below. 

<p align="center">
  <img src="/assets/cf_confidence.png" alt="CF results" width="100%"/>
</p>


## Cyber Physical Systems

### Carla PID Controller
|PID|Carla|Autonomous Driving|  

[See project on GitHub](https://github.com/burnsaustin145/carla_PID){:target="_blank"}

<p align="center">
  <img src="/assets/carla_ex.png" alt="CF makeup" width="100%"/>
  <em>Carla environment.</em>
</p>

A proportional-integral-derivative controller was created and tuned for car throttle and brake control. Using object detection sensors alone I was able to create a system which navigates in heavy traffic without collisions. 

<p align="center">
  <img src="/assets/states1.png" alt="CF makeup" width="100%"/>
  <em>A state transition diagram of the system.</em>
</p>

This system uses a waypoint selection module to plan a route, and then uses object detection to avoid collisions. The PID provides a way for the vehicle to maintain speed at a given set-point, and allows the vehicle to achieve set-point speed smoothly after a braking event.

Without tuning, we see the vehicle speed overshoots the orange line representing the given set-point. 

<p align="center">
  <img src="/assets/after_overshoot_tran.png" alt="CF makeup" width="100%"/>
  <em>Overshoot after braking event</em>
</p>

After tuning, we were able to smooth out the speed after a braking event.

<p align="center">
  <img src="/assets/clamp1.png" alt="CF makeup" width="100%"/>
  <em>We see the final result of speed over time, with minimal overshoot or oscillation</em>
</p>


### Detroit Crime Heatmap
|Graphical Statistics|  

[See project on GitHub](https://github.com/burnsaustin145/Heat-Map){:target="_blank"}  

This heatmap was created in R to visualize crime in Detroit over the last 100 years. 

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
### Haskell Based Semantic Network 
|Haskell|AI|  
This structure allows inferences to be made on semantic relations, as implemented in [this](https://github.com/burnsaustin145/SemanticGraph){:target="_blank"} Haskell project. 

This program performs the following operations

- add node_name -> adds a node to the graph
- relation domain_node relation range_node -> creates a labeled edge
- query range_node -> returns all domain nodes with range_node in the range
- infer node1 node2 -> creates a hypernode with label 'node1.node2', where the edges are the intersection of node1 edges and node2 edges
- reveal -> shows the current state of the graph