<p align="right">
  <a href="https://npmjs.org/package/react-map-gl">
    <img src="https://img.shields.io/npm/v/react-map-gl.svg?style=flat-square" alt="version" />
  </a>
  <a href="https://github.com/visgl/react-map-gl/actions?query=workflow%3Atest+branch%3Amaster">
    <img src="https://github.com/visgl/react-map-gl/workflows/test/badge.svg?branch=master" alt="build" />
  <a href="https://npmjs.org/package/react-map-gl">
    <img src="https://img.shields.io/npm/dm/react-map-gl.svg?style=flat-square" alt="downloads" />
  </a>
</p>

<h1 align="center">react-map-gl | <a href="https://visgl.github.io/react-map-gl">Docs</a></h1>

`react-map-gl` is a suite of [React](https://react.dev/) components designed to provide a React API for [mapbox-gl](https://github.com/mapbox/mapbox-gl-js) or [maplibre-gl](https://maplibre.org/maplibre-gl-js/docs/). More information in the online documentation.

See our [Design Philosophy](docs/README.md#design-philosophy).

### Installation

Using `react-map-gl` requires `react >= 16.3`.

```sh
# Using Maplibre
npm install react-map-gl maplibre-gl
```
_or_

```sh
# Using Mapbox
npm install react-map-gl mapbox-gl
```

### Example

```js
// Using Maplibre
import * as React from 'react';
import Map from 'react-map-gl/maplibre';
import 'maplibre-gl/dist/maplibre-gl.css';

function App() {
  return (
    <Map
      initialViewState={{
        longitude: -122.4,
        latitude: 37.8,
        zoom: 14
      }}
      style={{width: 600, height: 400}}
      mapStyle="https://api.maptiler.com/maps/streets/style.json?key=<Maptiler access token>"
    />
  );
}
```
_or_

```js
// Using Mapbox
import * as React from 'react';
import Map from 'react-map-gl/mapbox';
import 'mapbox-gl/dist/mapbox-gl.css';

function App() {
  return (
    <Map
      // https://visgl.github.io/react-map-gl/docs/get-started/mapbox-tokens
      mapboxAccessToken="<Mapbox access token>"
      initialViewState={{
        longitude: -100,
        latitude: 40,
        zoom: 3.5
      }}
      style={{width: 600, height: 400}}
      mapStyle="mapbox://styles/mapbox/streets-v9"
    />
  );
}
```

Learn more with in our [Getting Started](https://visgl.github.io/react-map-gl/docs/get-started) guide.


### Contribute

See [contribution guide](/CONTRIBUTING.md).


### Attributions

react-map-gl is part of vis.gl, an [OpenJS Foundation](https://openjsf.org) project.

Development is also supported by

<img src="https://raw.githubusercontent.com/visgl/deck.gl-data/master/images/branding/mapbox.svg" height="40" />
