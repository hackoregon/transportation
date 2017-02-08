# Transportation Alpha Spec

**TODO: describe goal for the alpha here**

## Frontend

* Landing page shows three layers from different datasets
* User can toggle each layer on/off
* User can click on a feature and view data from that feature
* User can *simluate* a new data submission:
  * User can draw line on map. 
  * Once line is complete a form UI will pop up with a textbox for entering data.
  * On submit, we can send a post request to http with geojson data for new feature

## Web API

Service APIs

```
GET / - list of data files  
GET /<id>.geojson - geojson file for datasets
GET /?source=<source>&bb=<bounding box>&daterange=<daterange>
```

## Backend Jobs

* Create three main Django models that will serve the APIs, one each for points, lines, and polygons.
* Rewrite/Create ingest scripts to transfer data from the stored json files to one of the three main tables.
* Create APIs to serve all data from three main models.
* Create APIs to filter data by date, source, and location.

