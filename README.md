# html-wcpms

An html component for Web Crop Phenology Metrics Service. 

This html file contains all the code needed to fetch a phenology metric from the web service [WCPMS](https://github.com/brazil-data-cube/wcpms.py) and with the return display a graph plot.

## Quick start

Add the `simple-wcpms.html` into the main app module of your project
```typescript
<div id="myPlot" style="width:100%;position:relative;height:100%"></div>
```
The code in the `<script>` will fetch the wcpms api for the phenology metrics and feed the dynamic graph with the metrics and time series ready for visualization.

The `html-wcpms` component 
![alt text](https://github.com/brazil-data-cube/html-wcpms/blob/master/examples/plot.png)

Then use the `collection`, `band`, `start_date`, `end_date`, `freq`, `latitude` and `longitude` variables to query the data to the display component
```typescript
var collection = "S2-16D-2";
var band = "NDVI";
var start_date = "2021-01-01";
var end_date = "2021-12-31";
var freq = "16D";
var latitude = "-11.749226797741814";
var longitude = "-45.75531005859376";
```



## Development

This project uses [Plotly](https://plotly.com/javascript/) version 3.0.1.
