# Fetch

TileFetch is a web application that allows users to select an area on a map, generate API links using the Google Solar API, and download the corresponding tiles (DSM, RGB, MASK) in a compressed ZIP file. The application provides a user-friendly interface, progress tracking, and detailed instructions for ease of use.

## Features

- **Interactive Map**: Use Leaflet.js to select an area by drawing a rectangle.
- **API Key Input**: Easily enter your Google API Key.
- **Generate Links**: Automatically generate API links for the selected area.
- **Download Tiles**: Download DSM, RGB, and MASK tiles as a ZIP file.
- **Progress Tracking**: Monitor download progress with a progress bar.
- **Loader Animation**: Visual indication while files are being downloaded.
- **Tooltips**: Contextual instructions for interactive elements.
- **Responsive Design**: Works well on both desktop and mobile devices.

## Getting Started

### Prerequisites

- **Google API Key**: You will need a Google API key to use the Google Solar API. You can get your API key from the Google Cloud Console.

## Usage

### Instructions

1. **Draw a Rectangle on the Map**:

   - Click on the rectangle icon in the top left corner of the map.
   - Click and drag on the map to create a rectangle around the area of interest.
2. **Enter Your API Key**:

   - Enter your Google API Key in the input box labeled "Enter your API key".
   - You can get your API key from the Google Cloud Console.
3. **Generate API Links**:

   - Click the "Generate API Links" button to generate the API links for the selected area.
   - The generated links will be displayed in the textarea below.
4. **Download Tiles**:

   - Click the "Download Tiles" button to start downloading the tiles.
   - The progress of the download will be shown in the progress bar.
   - Once completed, a ZIP file containing the tiles will be downloaded to your computer.

### Screenshots

#### Main Interface

#### Progress Bar

## Technologies Used

- **HTML/CSS**: For structure and styling.
- **JavaScript**: For functionality and interaction.
- **Leaflet.js**: For the interactive map.
- **Leaflet Draw**: For drawing rectangles on the map.
- **Leaflet Control Geocoder**: For geocoding and address search.
- **JSZip**: For creating ZIP files.
- **FileSaver.js**: For saving files to the user's computer.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgements

- [Leaflet.js](https://leafletjs.com/)
- [Leaflet Draw](https://github.com/Leaflet/Leaflet.draw)
- [Leaflet Control Geocoder](https://github.com/perliedman/leaflet-control-geocoder)
- JSZip
- [FileSaver.js](https://github.com/eligrey/FileSaver.js/)
