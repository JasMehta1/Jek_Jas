---
name: Data Visualization Assignment 8
tools: [Python, HTML, vega-lite]
image: assets/pngs/assignment8.png
description: This is a visualization for Assignment 8.2 
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# DV ASSIGNMENT 


<vegachart schema-url="{{ site.baseurl }}/assets/json/plot1.json" style="width: 100%"></vegachart>



#### Description of Visualization of PLOT 1:
-In this visualization, I am presenting the number of buildings by county and their respective statuses using a bar chart. The x-axis represents the counties, while the y-axis displays the count of buildings. The color of the bars indicates the status of the buildings, such as active, inactive, or under construction. By encoding the building status with color, viewers can easily distinguish between different statuses within each county.

-Design Choices:

-Encoding Types: I chose a bar chart for this visualization as it effectively represents the count of buildings in each county. The x-axis is assigned the nominal variable County, while the y-axis utilizes the aggregate function count() to represent the number of buildings.
-Color Scheme: The color encoding is used to differentiate between different building statuses. For example, active buildings might be represented in green, while inactive buildings could be represented in red. This color scheme was chosen to provide a clear visual distinction between the statuses and aid in the interpretation of the data.

-Data Transformations:
-No significant data transformations were performed for this visualization. The data was simply aggregated by county and building status to calculate the count of buildings for each category.

-Interactivity:
-Basic interactivity such as pan and zoom is enabled to allow users to explore the chart more easily. This feature facilitates a more interactive exploration experience, enabling users to focus on specific areas of interest within the visualization.



<vegachart schema-url="{{ site.baseurl }}/assets/json/plot2.json" style="width: 100%"></vegachart>


#### Description of Visualization of PLOT 2:
-Visualization 2: Square Footage of Buildings Over Time by Usage

-This visualization depicts the square footage of buildings over time, categorized by their respective usage descriptions. A scatter plot is utilized to represent the data, with the x-axis denoting the year of acquisition and the y-axis representing the square footage of buildings. Each data point is color-coded based on the usage description of the building. By leveraging color to encode the usage descriptions, viewers can easily discern between different categories of building usage.

-Design Choices:
-Encoding Types: A scatter plot was chosen for this visualization as it effectively displays the distribution of square footage over time. The x-axis is assigned the ordinal variable Year Acquired, while the quantitative variable Square Footage is mapped to the y-axis. Color encoding is utilized to differentiate between various usage descriptions, aiding in the identification of different building usage categories.
-Color Scheme: The color scheme employed in this visualization serves to distinguish between different usage descriptions. For instance, residential buildings may be represented in blue, while commercial buildings could be depicted in orange. This color scheme was selected to provide a clear visual differentiation between the usage categories and facilitate better interpretation of the data.

-Data Transformations:
-No significant data transformations were conducted for this visualization. The data was filtered based on the selected usage descriptions using interactive selection tools, allowing users to dynamically focus on specific categories of buildings.

-Interactivity:
Enhanced interactivity is integrated into the scatter plot to facilitate a more engaging exploration experience. Users can employ a selection tool to filter the data based on their chosen usage descriptions, enabling a more focused analysis of specific building categories over time. Additionally, an interactive brush selection feature is incorporated to allow users to dynamically select a range of years, further refining the exploration process and enabling deeper insights into the temporal trends of building square footage.
  
<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/JasMehta1/Jek_Jas/blob/main/python_notebooks/Workbook-2.ipynb" text="The Analysis" %}
</div>
