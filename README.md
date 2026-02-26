# Political-Data

## Overview

Political-Data is a **Live Election Results Dashboard** that visualizes election results from multiple countries and legislative bodies. The application displays seat distributions by party, shows majority requirements, and provides an interactive interface for exploring electoral data.

## Features

- **Interactive Charts**: Visual representation of election results using Highcharts item series
- **Multi-Country Support**: Browse election data from different countries and legislative bodies
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Real-time Data**: Fetches election data from Google Sheets
- **Party Information**: Displays each party's ideology group and seat count
- **Majority Indicator**: Shows the total seats and majority requirement needed
- **Color-Coded Parties**: Each party is displayed with its custom color

## Project Structure

```
Political-Data/
├── index.html                    # Main election results dashboard
├── README.md                     # This file
└── Standalone Application/
    └── index.html               # Standalone version of the dashboard
```

## How to Use

### Main Dashboard
1. Open `index.html` in a web browser
2. The dashboard will automatically load election data from Google Sheets
3. Select different countries and legislative bodies using the buttons
4. View the seat distribution and majority information

### Standalone Application
- Located in the `Standalone Application` folder
- Independent version of the dashboard with the same functionality

## Data Format

The application expects election data in CSV format from Google Sheets with the following columns:

| Column | Description |
|--------|-------------|
| Country | Name of the country |
| Body | Name of the legislative body (e.g., Chamber of Deputies, Senate) |
| Total Seats | Total number of seats in the legislature |
| Year | Election year |
| Party | Name of the political party |
| Seats | Number of seats won by the party |
| Ideology Group | Political ideology classification |
| Color Hex | Hex color code for party visualization |

## Technical Details

- **Framework**: HTML5, CSS3, JavaScript
- **Visualization Library**: [Highcharts](https://www.highcharts.com/)
- **Data Source**: Google Sheets (CSV export)
- **Browser Compatible**: All modern browsers

## Key Functionality

### Data Loading
- Automatically fetches election data from a configured Google Sheets URL
- Displays loading status and error messages
- Parses CSV data and converts it to structured JSON objects

### Interactive Selection
- Dynamic country selection through buttons
- Legislature type selection for each country
- Auto-selects the first available option on page load
- URL parameter support for direct country filtering

### Chart Rendering
- Semicircular item chart showing seat distribution
- Majority requirement line indicator
- Responsive sizing based on screen width
- Legend with seat counts for each party

### Responsive Layout
- Optimized for screens up to 480px width
- Adjustable font sizes and spacing for mobile devices
- Touch-friendly button controls

## Browser Requirements

- Modern JavaScript support (ES6+)
- HTMLCanvas or SVG rendering
- CORS enabled for Google Sheets access

## Future Enhancements

- Coalition analysis tools
- Historical trend comparison
- Export functionality
- Additional visualization options
- Real-time data polling

## About

This project was developed by the Center for Research Computing at Rice University to provide accessible visualizations of international electoral data.
