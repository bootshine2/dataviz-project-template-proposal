# Data Visualization Project

## Data

The data I propose to visualize for my project is the data that shows the number of bee colonies, beekeepers, and loss of bee colonies over time by US state and by year. The data can be found at: https://gist.github.com/bootshine2/ba15d3cb38e2ed31129aeca403405a12. It is duplicated from original pulication at [Data World (Bee Colony Loss.xlsx)](https://data.world/finley/bee-colony-statistical-data-from-1987-2017/workspace/file?filename=Bee+Colony+Loss.xlsx). It is statistical data from 1987 - 2017. The data provides information on (by state) the loss of bee colonies (by percent) annually, the number of known colonies, the number of known beekeepers, and the percentage of beekeepers exclusive to the state.

## Prototypes

I’ve created proof of concept visualizations of this data. The first is a US map that shows the loss of bee colonies by state on a geographic (US states) map that varies in color within state shading to show heavier or lighter bee colony loss. The second, third, and fourth are the variance of bee colony count, beekeeper count, and bee colony loss by state and by year in a heatmap. For visual referene, I would like to create a fifth, sixth and seventh visualization that are the same data as the previous 3 visualizations, but in a multitiered sunburst visualization, in order to see if any patterns better emerge there.

[![image](https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/us.png?raw=true)]https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/us.png?raw=true

[![image](https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/heatmapBeeLoss.png?raw=true)]https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/heatmapBeeLoss.png?raw=true

(please put a screenshot of one or more visualizations of this dataset you already made, for previous assignments)

## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:

 * How does the loss of bee colonies vary by state across years?
 * How does the number of bee colonies counted by census by state vary across years?
 * How does the number of beekeepers counted by census by state vary across years?
 * Is there any correlation between the above three statistics that shows or causes trends over time?

## Sketches

(insert one or more hand-drawn sketches of interactive visualizations that you imagine)
The first sketch is a US Map that shows loss by state over time of bee colonies.
[![image](https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/BeeLossByStatebyyear.png?raw=true)]
https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/BeeLossByStatebyyear.png?raw=true

The second sketch shows a heatmap used for the 3 types of data by state and by year--bee colony loss (in percent), number of colonies, and number of beekeepers.
[![image](https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/Bees1.jpg?raw=true)]
https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/Bees1.jpg?raw=true

The third sketch shows the same data in sunburst diagrams, in order to determine if the visual representation provides additional insight.
[![image]()]


## Open Questions

Describe any fear, uncertainty, or doubt you’re having about the feasibility of implementing the sketched system: I have figured out how to create basic plots using Vega-Lite and D3.js with React by following along, but I don't truly have a grasp on the available options for making new drawings. I would like to produce a US map that shows the states with color shading from green to red (green for good and red for bad) across time for bee colony loss, but I don't know how to: render the US states, and shade the states across time.
