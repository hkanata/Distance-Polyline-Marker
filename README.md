# Distance-Polyline-Marker

Calculate distance from polyline and marker

## Getting Started

You can calculate the distance between marker and polyline

### Run

Follow the steps below

Calling the main function

```
bdccGeoDistanceToPolyMtrs(Polyline, MarkerPosition);
```

example:

```
var coordinates = [
	{lat: 40.648501, lng: -73.975123},
	{lat: 40.598007, lng: -73.965295},
	{lat: 40.598349, lng: -73.961343},
	{lat: 40.602979, lng: -73.961469},
	{lat: 40.604613, lng: -73.947507},
	{lat: 40.619029, lng: -73.950297},
];
var polyline = new google.maps.Polyline({
	path: coordinates,
	geodesic: true,
	strokeColor: '#FF0000',
	strokeOpacity: 1.0,
	strokeWeight: 5
});

var marker = new google.maps.Marker({
	position: {lat: 40.62136542727805, lng: -73.96257983477432},
	map: map,
	title: 'Hello World!'
});

bdccGeoDistanceToPolyMtrs(polyline, marker.getPosition());

```

## Authors

* **hkanata** - *Initial work* - [PurpleBooth](https://github.com/hkanata)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
