# dokophoto (写真からどこ行くの？)

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)


![dokophoto collage banner](ss.jpg)


Discover nearby points of interest through a visual, photo-first interface. Dokophoto uses your current location to fetch and display a masonry grid of photos from local tourist spots and civic facilities. Tap a photo to see details, view it on a map, and get directions.

## Demo

**[Try the live demo](http://fukuno.jig.jp/1575)**

## Features

-   **Geolocation-based Discovery:** Automatically detects your location to find nearby attractions.
-   **Visual Photo Grid:** Displays attractions in a responsive, multi-column photo layout.
-   **Detailed Information View:** Tap any photo to open an overlay with the location's name, description, and other available data.
-   **Integrated Mapping:** Shows a static map with your current position and the destination's location.
-   **One-Tap Directions:** Provides a direct link to Google Maps for turn-by-turn navigation.
-   **Open Data Powered:** Utilizes linked open data from Japan's Open Data Platform.

## How It Works

The application retrieves the user's coordinates via the browser's Geolocation API. It then constructs a GeoSPARQL query to find nearby points of interest (specifically `TourSpot` and `CivicPOI` types) within a geographical bounding box. This query is sent to the jig.jp Open Data Platform (ODP) SPARQL endpoint, and the results, including image URLs and metadata, are dynamically rendered into the photo grid.

## Usage

1.  Open the [web application](http://fukuno.jig.jp/1575) in your browser.
2.  Allow the app to access your location when prompted.
3.  Browse the displayed photos and tap on them to view more details and get directions.

## Requirements

This project requires a modern web browser with JavaScript enabled and support for the Geolocation API.

## Data / API

The application uses the [jig.jp Open Data Platform (ODP) SPARQL endpoint](https://sparql.odp.jig.jp/data/sparql) to retrieve location data and photos.

## License

MIT License — see [LICENSE](LICENSE).