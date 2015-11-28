# map-dashboard
A dashboard of [Nashville building permits](http://data.nashville.gov/resource/3h5w-q8b7.json?) for fall 2015. A demo of the dashboard can be found [here](http://wallinm1.github.io/map-dashboard/).

This project is an exploration of adding a `Leaflet`-map and an interactive `DataTable`-table as filters in a `dc.js`-dashboard. With the help of the [`dc.leaflet`](https://github.com/dc-js/dc.leaflet.js)-plugin by [yurukov](https://github.com/yurukov) and [gordonwoodhull](https://github.com/gordonwoodhull), the integration of the new addons was rather painless. Using the interactive `DataTables`-tables does, however, seem to make the dashboard slightly less responsive. If performance is a concern, it is probably better to stick to the vanilla `dc.dataTable`.

The dashboard is largely a combination of ideas found in other tutorials and implementations:

* [The Nashville Building Permits-dashboard](https://github.com/cmvee/Nashville-Building-Permits) by [cmvee](https://github.com/cmvee)
* [The Beer Drinking Visualization-dashboard and tutorial](https://github.com/austinlyons/dcjs-leaflet-untappd) by [Austin Lyons](https://github.com/austinlyons)
* [The Earthquake Data Discovery-dashboard](http://bl.ocks.org/d3noob/6077996) by [d3noob](d3noob.org)
* The [Integrate with DataTables.js issue thread](https://github.com/dc-js/dc.js/issues/966) on the `dc.js` Github page.
* [This](http://stackoverflow.com/questions/21113513/dcjs-reorder-datatable-by-column/21116676#21116676) Stack Overflow-post
* [This](http://www.integritywatch.eu/) filterable `dc.js`-dashboard by the EU Integrity Watch and [tttp](https://github.com/tttp)

#### Updates 28.11.2015
* Added the `purpose`-field of the dataset as a clickable row detail and made the datatable searchable on that field.
* Fixed a bug that caused DataTables to display a warning message for text searches that return empty selections by defining a `defaultContent`-parameter for all columns.