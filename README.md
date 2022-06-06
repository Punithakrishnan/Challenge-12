## Challenge-12 -Plotly_Webpage
---
### Overview
---
In this project, I built an interactive dashboard to explore the Belly Button Biodiversity dataset, which catalogs the microbes that colonize human navels. 
The dataset reveals that a small handful of microbial species (also called operational taxonomic units, or OTUs, in the study) were present in more than 70% of people, while the rest were relatively rare. The dashboard includes a gauge chart, bubble chart, horizontal bar chart, and a summary of the metadata for the human that the sample came from.

### Using the Final Application

The application can be reached at https://punithakrishnan.github.io/Challenge-12/ and is hosted on Github Pages. When opening the dashboard, you see a view like this:
<img width="1318" alt="Screen Shot 2022-06-06 at 3 51 16 PM" src="https://user-images.githubusercontent.com/98849217/172237063-68c57af8-6c92-49a4-aa45-698ea618d149.png">

You are then able to scroll down for the full dashboard view that includes the bubble chart:
<img width="1293" alt="Screen Shot 2022-06-06 at 3 52 09 PM" src="https://user-images.githubusercontent.com/98849217/172237222-5e90bd7e-be56-41d0-9827-e2a68b4030b2.png">

The application is quite simple to use from there, select the Subject ID that you want to analyze in the dropdown and all of the charts and demographic info will populate with the proper data.

---
### Sotware Tools Used

These are the tools, techniques, and resources used in this project.

Plotly is used in combination with D3 and Javascript to generate the plots

HTML is used for the framework of the page

Github Pages is used to host the data and final application

The data is stored in JSON format and imported in

---
### About the Data

Hulcr, J. et al.(2012) A Jungle in There: Bacteria in Belly Buttons are Highly Diverse, but Predictable. Retrieved from: http://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/

---

### Project Steps

---
#### Page Layout and Logic

For page layout, I decided to stick with the html that was provided in the StarterCode. I beleive that this is quite an effective layout for a dashboard and it provides proper spacing for each figure.

The javascript logic is what took me the most time. After realizing that the page needs a "master function" that calls in the data and updates all of the charts, the project became a little easier.

### Code Layout

The first thing that happens is a call to the json data which is used to populate the dropdown. Once that is populated, the optionChanged function is called. This function also connects to the json, but for different data, it then uses that data to run the other 4 functions that populate the bar chart, gauge chart, Demographic Info div, and the bubble chart. This function is also called in the html whenever the value of the dropdown is changed.

### Bar Chart

<img width="694" alt="Screen Shot 2022-06-06 at 3 56 58 PM" src="https://user-images.githubusercontent.com/98849217/172237973-0b3290dc-29b7-4b01-98c1-883670f01886.png">

The code for the bar chart is extremely simple, with no manipulation at all. It is a generic plotly horizontal bar chart. The 'text' parameter is used for adding text to the labels on hover.

---

### Bubble chart 
---

<img width="1205" alt="Screen Shot 2022-06-06 at 4 00 42 PM" src="https://user-images.githubusercontent.com/98849217/172238543-31697424-c810-4a30-9c67-6e29eb4f565e.png">


### gauge plot
---

<img width="598" alt="Screen Shot 2022-06-06 at 4 01 18 PM" src="https://user-images.githubusercontent.com/98849217/172238630-5e91076f-e9cb-4ddd-b20d-fa4704d65bfb.png">



