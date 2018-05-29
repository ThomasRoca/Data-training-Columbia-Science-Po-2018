# Data access in the 21st century
**May the 29th 2018, Columbia Univ. Science-Po 2018**
*Thomas Roca, PhD, Data Strategist Microsoft*

Stay in touch via [Twitter](https://twitter.com/Thomas_Roca), [Github](https://github.com/ThomasRoca/) or [LinkedIn](https://www.linkedin.com/in/thomas-roca-43347484/)

Lecture will be available here [Link to the lecture]

<br>

**If not yet done, take the [Data Skills Survey](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRxKuu6TlN1dBuJsnZlxRHxFUNExXOUpTVjNTM05CSEdZSlRISzFCNFJRVi4u)**

---

**Tools we are going to use:**

For this workshop, you will need to install a **code editor**:
- e.g. [Visual Studio Code](https://sourceforge.net/projects/vscode-portable/);

We are also going to use: 
- 	**JSFiddle**, a javascript online editor [sign up here - free](https://jsfiddle.net/user/signup/)
-  **Jupyter Notebook**, Microsoft Azure proposes an online Notebook that does not require python to be on your machine: [sign up- free](https://notebooks.azure.com/)

## Content
**Part 1: 1h30**

I. Intro: Data flows in the information age (30 min)
- Data infrastructure
- Machine's way to store data

II. Accessing data from networks (1h)
- API the programmatic way to share and access data
- API: provides data and services
- Algorithm and Machine Learning as a Service
  - [Example Sentiment analysis](https://pythonappcela.azurewebsites.net/sentiment_analysis)
  - [Faces and Emotion detection](http://pythonappcela.azurewebsites.net/computer_vision)
 
--- 
**Part 2: 2h00**

III. Cloud computing and AI: The Microsoft Framrework (30min)

IV. Hands on! Mining data from networks (1h30)

**To do learn list**

- Scarpping the web: 
	- from the browser: **try to extract data from your internet browser using the console and draw a graph using [highcharts](https://jsfiddle.net/ThomasRoca/rkbz7fhb/87/)**
	- The proper way to scrap data: **Example with [python](https://notebooks.azure.com/ThomasMSFT/libraries/Tutorial/html/Scrap%20data%20from%20the%20web.ipynb)** 
- [Hello World ! Make a call to World Bank api](https://jsfiddle.net/ThomasRoca/j5d919k4/)
- Hands-on 1: [Make your first connected dataviz with Highcharts and World Bank API](https://www.highcharts.com/demo/line-basic) 

**To do list**

- Hands-on 2.1: Scraping Airparif with Python
	- **Try to adapt the python example to get data from Aiparif and build a bar chart to display airquality in Paris for yesterday, today and tomorrow. [Link](https://www.airparif.asso.fr/rss/indices)**
- Hands-on 2.2: Using API e.g. [Pollution in Amaravati](http://jsfiddle.net/ThomasRoca/bLbz5oqd/)

---


## Link from the presentation: 
- [Reading a local JSON in JavaScript](https://jsfiddle.net/ThomasRoca/ss0wq9oq/14/)
- API call to the world Bank WDI
	- [https://api.worldbank.org/v2/countries/VNM/indicators/AG.LND.ARBL.ZS?per_page=5&MRV=5&format=json](https://api.worldbank.org/v2/countries/VNM/indicators/AG.LND.ARBL.ZS?per_page=5&MRV=5&format=json)
	- [JSFiddle call to the API](https://jsfiddle.net/ThomasRoca/4gjfs1h2)
- Getting real time pollution data in India: 
	- End point of the API: https://api.data.gov.in/resource/3b01bcb8-0b14-4abf-b6f2-c1bfd384ba69?api-key=579b464db66ec23bdd000001cdd3946e44ce4aad7209ff7b23ac571b&format=json&offset=0&limit=7
- [Data application](https://jsfiddle.net/ThomasRoca/1vpypyc9/)
- [Wikipedia page for Asia](https://en.wikipedia.org/wiki/Asia)
- **JavaScript to scrap from the browser**
	```// Select an object and get its ID here:  GDP table id is dollar 0: $0
	var Table = $$("tr", $0)
	// Read first cell
	Table[0].cells[0].innerText
	// create an empty array
	var array=[];
	// loop
	for(i=0; i<Table.length; i++) {
	array[i]={name:"", data:[]};
	//Copy the first column
	array[i].name=Table[i].cells[1].innerText;
	//Copy the second column
	array[i].data=[parseFloat(Table[i].cells[2].innerText.replace(/[^\d\.\-]/g, ""))]
	}
	copy(array)
	```
	
---

# More resources

### Further reading:
- Friendly, M., 1999, "Re-Visions of Minard", [link](http://www.datavis.ca/gallery/minard/minard.pdf])
- Friendly, M., 2008, "A Brief History of Data Visualization" [link](http://byrneslab.net/classes/biol607/readings/Friendly_2008_dataviz_history.pdf)
- Lupi, H., Posavec, S.,2016, "Dear Data", http://www.dear-data.com/
- Yau, N. 2011, visualize this: the flowingdata guide to design, visualization, and statistics [link](http://book.flowingdata.com)
- The Smithonianmag:"The Revolutionary Infographics of W.E.B. Du Bois And Booker T. Washington" [link](http://www.smithsonianmag.com/smart-news/the-revolutionary-infographics-of-web-du-bois-and-booker-t-washington-180959756)
- ToucanTouco, Infographie vs Dataviz: Faites la différence. [Link](https://toucantoco.com/blog/infographie-vs-dataviz/)
- Tufte, E. R. The Visual Display of Quantitative Information. Graphics Press, Cheshire, CT, 1983.
- Hagley, J. What is the difference bewteen infographic and dataviz ? [Link](http://www.jackhagley.com/What-s-the-difference-between-an-Infographic-and-a-Data-Visualisation)

### Tutorials

**Tuto I wrote for Highcharts**
- [Open Data API for Chart Creation part1](https://www.highcharts.com/blog/data-science/233-world-bank-open-data-api-highcharts-part1/)
- [Open Data API for Chart Creation part2](https://www.highcharts.com/blog/post/235-open-data-api-for-chart-creation-part-2/)

- **online tools**
	- [Pick your color](https://www.w3schools.com/colors/colors_picker.asp) with [Color brewer](http://colorbrewer2.org)
	- Read your JSON with [jsoneditoronline.org](http://jsoneditoronline.org/)
	- store your JSON with [myjon.com](http://myjson.com/)
	- Convert shapefile to GeoJSON with [mygeodata](https://mygeodata.cloud/)
	
- **Code sample we saw on JSfiddle**:
	- [SVG](http://jsfiddle.net/ThomasRoca/q754amnd/)
	- [highcharts](http://jsfiddle.net/ThomasRoca/fps87ooa)
	- [leaflet](http://leafletjs.com/examples/quick-start/example-popups.html)
	- [Javascript](http://jsfiddle.net/ThomasRoca/50snpv6r/)
	- [Interaction](https://jsfiddle.net/ThomasRoca/vuw7grwL/)
	- [parse JSON data](http://jsfiddle.net/ThomasRoca/5f4jh80c)
	- [How to make an API Call](https://jsfiddle.net/ThomasRoca/j5d919k4/3/)
	- [Draw a graph with from API data](https://jsfiddle.net/ThomasRoca/pxmxpsed/2/)
	- James' graph! Call Api, user interface and graph [link](https://jsfiddle.net/jegiles/ddffgz29/)
	- [DHS API with leaflet](http://jsfiddle.net/ThomasRoca/069Lqfkz/?utm_source=website&utm_medium=embed&utm_campaign=069Lqfkz)

- **Highcharts:**
	- https://www.highcharts.com/demo
	- https://www.highcharts.com/blog/
- **HTML, CSS and JS:** 
	- https://www.w3schools.com

- [Data Glossary - Data-Pop Alliance](https://github.com/ThomasRoca/Lecture-Columbia-Science-Po-2017/blob/master/Glossary.md)
- [Mapping Data Sources for development](https://afdlab4dev.github.io/Wiki-DataExploration-in-AFD/)

