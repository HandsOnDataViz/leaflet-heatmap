# Leaflet Heatmap template
This map uses a [Leaflet.Heat](https://github.com/Leaflet/Leaflet.heat) plugin
to transform points into a heat layer.

![Screenshot](screenshot.png)

## Demo
https://handsondataviz.github.io/leaflet-heatmap

Sample data by the [Metropolitan Police Service](https://data.police.uk/data/) for January–July 2020.

## Make your own

1. Press **Use this template** button to create a copy of this repository in your own GitHub account.
2. Modify map's title and description inside `index.html`.
3. Put your point coordinates data inside `data.csv`. Don't use a header, and keep it one point per line.
Use *latitude,longitude* (or *y,x*) order, like below:
```
51.506585,-0.139387
51.505467,-0.14655
51.507758,-0.141284
```
4. Depending on your data density, you might want to tweak `radius` and `blur` parameters inside `<script>` of `index.html`:
```javascript
  var heat = L.heatLayer(data, {
    radius: 25,
    blur: 15,
  })
```

For more information on customization, see [Leaflet documentation](https://leafletjs.com/).

## See other Leaflet templates
* [Simple Leaflet map](https://github.com/HandsOnDataViz/leaflet-map-simple)
* [Leaflet map with CSV data](https://github.com/HandsOnDataViz/leaflet-map-csv)
* [Leaflet map with open data APIs](https://github.com/HandsOnDataViz/leaflet-maps-open-data-apis)
* [Leaflet map with data from Socrata](https://github.com/HandsOnDataViz/leaflet-socrata)
* [Leaflet polygon map with tabs](https://github.com/HandsOnDataViz/leaflet-map-polygon-tabs)
* [Searcheable Map Template](https://github.com/HandsOnDataViz/searchable-map-template-csv)
* [Leaflet Maps with Google Sheets](https://github.com/HandsOnDataViz/leaflet-maps-with-google-sheets)
* [Leaflet Storymaps with Google Sheets](https://github.com/HandsOnDataViz/leaflet-storymaps-with-google-sheets)
