
# Notes #

**Rough Outline**

* Introduction to [Leaflet.js](https://leafletjs.com/)
* A site of mine with an [example](http://maps.johnfmarion.com/)
* `example1.html`: The Quick Start Example
* `example1.html` with commented block included
* HTML5 Geolocation in browser console.
* `example2.html`: User's current location.
* Discussion of map projection and zoom levels
  * http://leafletjs.com/examples/zoom-levels/
* Network Tab Analysis: The PNG Requests with x/y/z
* Discussion of custom tiles (either from server or class extension)
  * http://leafletjs.com/examples/extending/extending-2-layers.html
* KML and GeoJSON: Samples included
* `example3.html`: Plotting the sample GeoJSON
* Styling and GeoJSON: http://leafletjs.com/examples/geojson/
* Mapbox Discussion
* Side Note: Leaflet is Mobile Friendly (http://leafletjs.com/examples/mobile/)
* Examination of the Jekyll Site
* Brainstorming Possible Projects:
  * A simple GPS App
  * A simple Weather Tracker (using some weather API)
  * A Risk-like Game
  * Plotting locational data
  * Server Side: Override some map tilesS

## HTML5 Geolocation #

```javascript
function geoCallback(pos) {
  console.log([pos.coords.latitude, pos.coords.longitude, pos.coords.accuracy, pos.timestamp]);
}
navigator.geolocation.getCurrentPosition(geoCallback);
```