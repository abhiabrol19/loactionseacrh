# Location Finder React Application

## Overview

The Location Finder React Application is a web app that allows users to search for locations and view them on an interactive map. Users can search for places, and the app will display the location on a map with a marker. The app is designed to be simple, responsive, and user-friendly.

## Key Technologies

- **React**
- **TypeScript**
- **React Hooks**
- **React Leaflet**: A library that integrates Leaflet maps into React, making it easy to display and interact with maps.
- **Leaflet**: A lightweight JavaScript library for interactive maps.
- **Nominatim API**: Used to search and fetch location data based on user input.
- **Tailwind CSS**: A utility-first CSS framework for building responsive and stylish UI components.

## Project Structure

### Main Entry Point

- **`main.tsx`**: Initializes the application and renders the root component (`App`) into the DOM, wrapped in `React.StrictMode` to ensure best practices.

### Core Components

- **App Component**:  
  - Combines the search and map functionalities.
  - Manages the selected location state.
  - Displays the `LocationSearch` and `Map` components in a two-column layout.

- **LocationSearch Component**:  
  - Allows users to search for locations.
  - Displays a list of search results.
  - Sends selected location data to the map when a location is clicked.

- **Map Component**:  
  - Displays the map and centers on the selected location.
  - Adds a marker to the map at the selected location's coordinates.

### API Integration

- **Nominatim Search API**:  
  - Fetches location data based on user input.
  - Returns coordinates and details of matching locations.

### State Management

- **React State Management**:  
  - `useState` is used to keep track of the selected location and update the map view accordingly.

### Styling

- **Tailwind CSS**:  
  - Provides utility classes for responsive design and easy styling.

## How the Application Works

1. **Application Launch**:  
   - The app displays a search section on the left and a map on the right.

2. **Searching for Locations**:  
   - Users enter a search term (e.g., a city or address) in the search box.
   - The app fetches matching locations from the Nominatim API.

3. **Displaying Search Results**:  
   - A list of found locations is displayed.
   - Users can select a location from the list to view it on the map.

4. **Map Visualization**:  
   - When a location is selected, the map centers on the location and displays a marker.

