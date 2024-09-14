# Canada Postsecondary Institutions Map

This project provides an interactive map of Canada showcasing postsecondary institutions and relevant data such as enrolment counts, unemployment rates, and student debt. The map allows users to explore and visualize data by province and year, with options to switch between different modes of data representation.

## Features

- **Interactive Map**: View and interact with a map of Canada, where each province is clickable to display additional information.
- **Year Controls**: Switch between different years to see how enrolment counts and other metrics change over time.
- **Data Modes**: Toggle between different data modes including enrolment, unemployment rates (all education levels, no postsecondary education, and postsecondary education).
- **Timeline Chart**: Display a timeline chart showing average student debt over time for a selected province.
- **Dynamic Updates**: The map updates dynamically based on the selected year and data mode.

## Data Sources

- **Canada GeoJSON**: GeoJSON file of Canada's provinces for map rendering.
- **Enrolment Data**: CSV file containing enrolment counts by province and year.
- **Unemployment Data**: CSV file with unemployment rates by province, broken down by education level.
- **Debt Data**: CSV file with average student debt by province and year.
- **Institutions Data**: CSV file listing postsecondary institutions with their geographic coordinates.

## Setup and Usage

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, etc.)
- Internet connection (for loading external data and libraries)

### Files

1. **HTML File**: Contains the structure of the map and user interface.
2. **CSS**: Embedded within the HTML file for styling.
3. **JavaScript**: Embedded within the HTML file for interactive functionality.

### Instructions
1. **Clone the Repository**: 
   ```bash
   git clone [REPOSITORY_URL]
   cd [REPOSITORY_DIRECTORY]
   ```

2. **Open `index.html`**: Open the `index.html` file in your preferred web browser.

3. **Data Files**: Ensure that the following data files are correctly referenced and available:
   - `province_enrolment.csv`
   - `province_unemployment.csv`
   - `province_debt.csv`
   - `institutions.csv`
   - `university.png` (Icon image for institutions)

4. **External Libraries**: The project uses [D3.js](https://d3js.org) for data visualization and map rendering. The library is loaded from a CDN in the HTML file.

### Features and Controls

- **Year Controls**: Select a year to update the map and data visualization. The active button will be highlighted.
- **Data Modes**: Select different data modes to view various types of information on the map. The map colors and icons will adjust accordingly.
- **Timeline Chart**: Click on a province on the map to display a chart of student debt over time. Use the "Close Chart" button to hide the chart.

## Development

### Adding Data

- Ensure data files are in the correct format (CSV) and follow the expected schema.
- Update the `d3.csv` calls in the JavaScript code to match the location of your data files if they are not in the same directory as `index.html`.

### Customization

- **Map Projection**: Adjust the `d3.geoMercator()` settings for different map projections or zoom levels.
- **Color Scales**: Modify the color scales for enrolment and unemployment to better fit your data range.
- **Icons and Styling**: Customize the icon image and CSS styles as needed.

## Troubleshooting

- **Data Loading Issues**: Check the console for errors related to data loading and ensure that the file paths are correct.
- **Map Rendering**: Verify that the GeoJSON file and projection settings are appropriate for the map visualization.

## License

This project is licensed under the [MIT License](LICENSE).

