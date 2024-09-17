# Greece Prefectures & Prefecture Units GeoJSON Data

This repository contains GeoJSON data files representing the prefectures and prefecture units of Greece. The data is structured for easy integration into applications that need geographic boundaries for regions and sub-regions across Greece.

## Features

- **GeoJSON Format**: All prefectures and prefecture units are represented as polygons, making them easy to visualize on maps.
- **Multi-language Support**: Prefecture names are available in both English and Greek (`name` and `name_greek` properties).
- **Unique Identifiers**: Each prefecture and prefecture unit is associated with a unique `id` for reference and programmatic access.

## File Structure

- `greecePrefectures.geojson`: Contains the boundaries for all Greek prefectures.
- `greecePrefecturesUnits.geojson`: Contains the boundaries for all Greek prefecture units (regional units).

### Example Properties in GeoJSON:
Each GeoJSON feature contains the following properties:
- `id`: Unique identifier for the prefecture/prefecture unit.
- `name`: Prefecture or prefecture unit name in English.
- `name_greek`: Prefecture or prefecture unit name in Greek.

### Example GeoJSON Feature:
```json
{
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [25.906707597593453, 41.307374753490606],
        [25.903924711171832, 41.306382733525446],
        ...
      ]
    ]
  },
  "properties": {
    "id": "0106",
    "name": "Rodopis",
    "name_greek": "Ροδόπης"
  }
}
```

## Usage

You can use the GeoJSON data in any mapping or geographic application that supports the format, such as:
- Google Maps
- Leaflet.js
- Mapbox
- GIS software

### How to Load GeoJSON:
You can easily load and display this data in mapping libraries like Leaflet or Mapbox:

```javascript
// Example using Leaflet
L.geoJSON(prefecturesData).addTo(map);
```

## Contribution

Contributions are welcome! If you have updated boundaries or additional data to include, feel free to submit a pull request or open an issue.

## License

This project is licensed under the MIT License. You are free to use and modify the data, but please give appropriate credit.
