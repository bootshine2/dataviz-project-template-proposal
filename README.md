# Data Visualization Project

## Data

The data I propose to visualize for my project is the data that shows the number of bee colonies, beekeepers, and loss of bee colonies over time by US state and by year. The data can be found at: https://gist.github.com/bootshine2/ba15d3cb38e2ed31129aeca403405a12. It is duplicated from original pulication at [Data World (Bee Colony Loss.xlsx)](https://data.world/finley/bee-colony-statistical-data-from-1987-2017/workspace/file?filename=Bee+Colony+Loss.xlsx). It is statistical data from 1987 - 2017. The data provides information on (by state) the loss of bee colonies (by percent) annually, the number of known colonies, the number of known beekeepers, and the percentage of beekeepers exclusive to the state.

## Prototypes

I’ve created proof of concept visualizations of this data. The first is a US map that shows the loss of bee colonies by state on a geographic (US states) map that varies in color within state shading to show heavier or lighter bee colony loss. The second, third, and fourth are the variance of bee colony count, beekeeper count, and bee colony loss by state and by year in a heatmap. For visual referene, I would like to create a fifth, sixth and seventh visualization that are the same data as the previous 3 visualizations, but in a multitiered sunburst visualization, in order to see if any patterns better emerge there.

[![image](https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/us.png)]https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/us.png

[![image](https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/heatmapBeeLoss.png?raw=true)]https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/heatmapBeeLoss.png?raw=true

## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:

 * How does the loss of bee colonies vary by state across years?
 * How does the number of bee colonies counted by census by state vary across years?
 * How does the number of beekeepers counted by census by state vary across years?
 * Is there any correlation between the above three statistics that shows or causes trends over time?
 * (added 10/2): Do particular states trend down or up in percent bee colony loss, number of beekeepers, or number of colonies?

## Sketches

(insert one or more hand-drawn sketches of interactive visualizations that you imagine)
The first sketch is a US Map that shows loss by state over time of bee colonies.
[![image](https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/BeeLossByStatebyyearWithDropdowns.png)]
https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/BeeLossByStatebyyearWithDropdowns.png

The second sketch shows a heatmap used for the 3 types of data by state and by year--bee colony loss (in percent), number of colonies, and number of beekeepers.
[![image](https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/Bees1wDropdowns.jpg)]
https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/Bees1wDropdowns.jpg

The third sketch shows the same data in sunburst diagrams, in order to determine if the visual representation provides additional insight.
[![image](https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/Bees2withDropDowns.jpg)]https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/Bees2withDropDowns.jpg


## Open Questions

Describe any fear, uncertainty, or doubt you’re having about the feasibility of implementing the sketched system: I have figured out how to create basic plots using Vega-Lite and D3.js with React by following along, but I don't truly have a grasp on the available options for making new drawings. I would like to produce a US map that shows the states with color shading from green to red (green for good and red for bad) across time for bee colony loss, but I don't know how to: render the US states, and shade the states across time.

## Schedule of Deliverables

* Make the interactive US map of bee colonies and loss 10/10
  * Make a D3.js heatmap
  * Tie data to the D3.js heatmap
  * Color the states by heatmapping for the selected field (colonies, beekeepers, or colony loss)
  * Add dropdowns to the page
    * Add dropdown to choose from: US map viz, heatmap, or sunburst
    * Add dropdown to choose selected data field to display: (colonies, beekeepers, or colony loss)
  * Make the page adjust based on dropdowns.
  (*Note that I am still working on the dropdown. Got the color right and made the legend fit.*)
  
  [![Image](https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/bee%20loss%20by%20year%202.PNG)](https://beta.vizhub.com/bootshine2/1ab048f3d6b14f91869d618fe70f1eb2?mode=full)

* Make the interactive US map of bee colonies and loss 10/17
  * Make a D3.js US states map
  * Tie data to the D3.js US states map
    * Create or determine data source. This should be a geoJSON topo map of the states.
    * Put the data in D3.js with React using AlbersUsa or other correct topo library.
  * Color the heatmap squares by heatmapping for the selected field (colonies, beekeepers, or colony loss)
  * Add dropdowns to the page
    * Add dropdown to choose from: US map viz, heatmap, or sunburst
    * Add dropdown to choose selected data field to display: (colonies, beekeepers, or colony loss)
  * Make the page adjust based on dropdowns.
  (*Colors are now right. still working on tooltips and dropdown. But I'm getting there...*)
  [![Image](https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/bee%20loss%20cloropleth.png)](https://beta.vizhub.com/bootshine2/daf80e80faf54d67a61de8f53e55506e?edit=files&file=index.js&mode=full)
  
* Make the interactive sunburst or dendritic of bee colonies and loss 10/24
  * Make a D3.js sunburst or dendritic
  * Tie data to the D3.js display
  * Color the arcs based on the selected field (colonies, beekeepers, or colony loss)
  * Add dropdowns to the page
    * Add dropdown to choose from: US map viz, heatmap, or sunburst
    * Add dropdown to choose selected data field to display: (colonies, beekeepers, or colony loss)
  * Make the page adjust based on dropdowns.
  (*Working on tne dropdowns still. But here is the treemap as opposed to the dendritic. *)
  [![Image](https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/treemap.png)](https://beta.vizhub.com/bootshine2/ada11d6edcc44b5ca57297f6c2acc879?edit=files&file=index.html&mode=full)
  
* Add narrative to the page and finalize 10/31
  * Show how the data helps the reader understand the answer to the questions
  * provide explanation of where the data came from and background on why the subject is important.
  
  This final week, I tried to add dropdown menus to my three major visualizations (multicolor scatterplot, chloropleth of bee data across US states, and treemap). I was able to get this working in one of them, shown here:
  [![Image](https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/BeeScatterPlotWithDropDown.jpg)](https://beta.vizhub.com/bootshine2/0a0b3a03537842a4bb256086ff85ca21?edit=files&file=index.js&mode=full)
  
  I tried to add the same code for the dropdown to the chloropleth after getting it to work with the scatterplot, but my lack of experience with JS Ecmascript 6 and also with D3 and React kept me from reaching my goal. Nevertheless, I added most of the code into the chloropleth already noted [here](https://beta.vizhub.com/bootshine2/daf80e80faf54d67a61de8f53e55506e?edit=files&file=index.js&mode=full). 
  
  Additionally, instead of the Treemap that I was able to make work and tie to my data, I intended to create a D3 sunburst. I was able to port code from an observablehq sunburst over to my page [here](https://beta.vizhub.com/bootshine2/762d08e3a7a746d3918e145b7b12aa95?edit=files&file=index.js&mode=full), but you'll notice from the picture below that it's the same data as from the original sunburst code example [here](https://observablehq.com/@d3/zoomable-sunburst).
  [![Image](https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/FailedSunburst.jpg)](https://beta.vizhub.com/bootshine2/762d08e3a7a746d3918e145b7b12aa95?edit=files&file=index.js&mode=full)
  
  I wasn't able to figure out how to get the code to pull my data, but I was able to use JS code to transpose my CSV file of bee colony loss data to the right form of JSON file using the code in VizHub at the following picture:
  [![Image](https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/JSONmaker.jpg)](https://beta.vizhub.com/bootshine2/beebcddb5fed4c7783b242816468ba9e)
  
## Narrative and exposition on what this data and these visualizations show, and why I chose to do this:

In reiteration, my data originally came from [Data World (Bee Colony Loss.xlsx)](https://data.world/finley/bee-colony-statistical-data-from-1987-2017/workspace/file?filename=Bee+Colony+Loss.xlsx). It is statistical data from 1987 - 2017. The data provides information on (by state) the loss of bee colonies (by percent) annually, the number of known colonies, the number of known beekeepers, and the percentage of beekeepers exclusive to the state.

I was really interested in bees, as my wife and I have considered starting a bee colony. We live on a river in Virginia and have the land and ability to start one. What I thought I would learn through the visualization of the data was that bees tend to colonize in particular areas of the US and that these areas either have remained reasonably constant or have shifted over time, but are not random. I also thought that the number of beekeepers would show the same trends, and that bee colony loss would as well. 

What I discovered from visualizing the data is that there are specific states (e.g., California), where the bee colonization is typically higher, but that this really doesn't show a good trend, and that bee colonization numbers are truly variable across the US. This is good news, I suppose, in understanding that I can start a bee colony in Virginia, and can further start a colony in another state if I were to move. What would be interesting would be to understand whether there is similarity in data associated with specific types of bees. Unfortunately, that level of detail data is not available.

I certainly hope you are able to take something away from this exposition! If you take one thing away, know that you can start a bee colony (under the right conditions) wherever you live!

## YouTube video of me explaining my project!
You can go [here](https://youtu.be/hljrKtjxKXQ) to see the video where I explain why I took on this project and what I went through to complete it. Hopefully it inspires someone to continue looking into data visualization and/or bee colonization!

![Image](https://github.com/bootshine2/dataviz-project-template-proposal/blob/master/face.PNG)
